Use active voice in documentation whenever possible. It improves readability by clearly identifying the subject performing the action. In instructional or procedural content, this structure makes tasks more straightforward:

✅ **Good:** Call the getSessionData() method before rendering the calendar.  
❌ **Bad:** The getSessionData() method should be called before rendering the calendar.

However, there are some situations where passive voice is preferred. For example:
* The object of the action is more important than the actor.
	* Example: The API key was revoked after 24 hours.
* Consistency is required across system documentation (e.g., API responses and success/error descriptions).
	* Example: A 403 status code is returned when the user is unauthorized.
* The action’s actor doesn’t matter (e.g., automated backend processes).
	* Example: The edit log will be updated automatically.