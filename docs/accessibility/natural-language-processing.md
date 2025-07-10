At WellnessLiving, customers interact with our platform through voice bots, chat prompts, and real-time call flows. Documenting these NLP-powered features requires clarity, context, and consistency.

## Prompt design and structure
* Use clearly defined roles: `system`, `user`, `assistant`.
* Always define a system prompt (e.g., “You are a helpful voice assistant for a fitness studio.”).
* Avoid vague or open-ended instructions.
* Support Markdown-safe formatting in both prompts and completions.

JSON example:
``` json
{
  "messages": [
    {"role": "system", "content": "You are a support agent."},
    {"role": "user", "content": "I need help rescheduling my class."}
  ]
}
```

## Tool calling and function definitions
* Define callable functions using consistent, self-descriptive names (e.g., `transfer_call`, `schedule_callback`).
* Every function should include typed arguments, error handling behavior, and a clear success message.
* Document fallback flows when functions are unavailable or calls fail.

Sample Python function:
```python
async def transfer_call(self, phone_number: str) -> Tuple[None, str]:
    """
    Transfer the current call to a human agent at the specified phone number.

    Args:
        phone_number (str): The phone number to transfer the call to.

    Returns:
        Tuple[None, str]: A tuple with `None` as the result, and a success or error message.
    """
    try:
        # Validate the phone number (simple check)
        if not phone_number.startswith("+"):
            raise ValueError("Phone number must be in E.164 format (e.g., +1234567890)")

        # Call LiveKit API to add the human agent to the call
        await self.livekit_client.create_sip_participant(phone_number)

        # Confirm success to the user
        await self.session.say("I'm transferring you to a human agent now. Please hold.")
        return None, f"Call successfully transferred to {phone_number}."

    except Exception as e:
        # Log the failure and notify the user
        await self.session.say("I'm sorry, I couldn't complete the transfer.")
        self.logger.error(f"Transfer failed: {e}")
        return None, f"Transfer failed: {str(e)}"
```

## Voice agent transitions
* When handing off to a human, include a spoken introduction (e.g., “Let me connect you to a human agent who can help.”).
* Maintain presence until the human joins; never drop the user unexpectedly.
* Use silence or hold music instead of re-prompting during transfer.

## Testing and monitoring
* Log prompt inputs and model outputs with timestamps.
* Track function-call usage and frequency of escalations.
* Set up spec-driven tests for NLP endpoint contracts and behavior.