Use **sentence case** throughout developer‑focused documentation. Capitalize only the first word of each heading, sentence, or phrase. Use **title case** or **uppercase** for proper nouns, branded names, and standard acronyms.

## Headings and section titles
Capitalize only the first word and any proper nouns.
* ✅ (good) Authentication error codes
* ❌ (bad) Authentication Error Codes

## API parameter descriptions
Use sentence case when writing parameter descriptions, whether in API tables or inline documentation. Descriptions should begin with a capitalized lexical item (usually a noun or adjective) and avoid unnecessary title casing of noun phrases or modifier strings.

Most parameter descriptions are noun phrases (not full clauses), and therefore do not require a final period unless they form a complete sentence. Capitalize only the first word of the phrase unless it includes proper nouns or acronyms.
* ✅ (good) client_id: Unique identifier for a client  
* ❌ (bad) client_id: Unique Identifier For A Client

The phrase “unique identifier for a client” is a noun phrase with prepositional modifier, not a sentence. Only the initial word (“unique”) is capitalized.

## Code comments and examples
Write comments and inline documentation in sentence case, even when embedded in code blocks. Most code comments are imperative clauses or noun phrases that describe actions or context; they aren't titles or headers, and they shouldn't use title case.

The first word of a comment is capitalized if it begins a new sentence or clause. Avoid capitalizing every word unless the comment is documenting a constant or mimicking external casing (like a class name). This helps maintain visual alignment with system messages, logs, and documentation strings.

✅ (good):
```python title="Python"
# Generate an access token
token = auth.generate_token()
```

❌ (bad):
```python title="Python"
# Generate An Access Token
token = auth.generate_token()
```

Even though the comment starts with a capitalized verb (“Generate”), the rest of the comment should remain in sentence case.

## Error messages
Error messages should follow sentence case and function as complete, grammatically correct sentences (typically in the indicative mood). Capitalize only the first word and any proper nouns or technical acronyms.

Most error messages are structured as either:
* A simple declarative sentence ("Timeout error: request took longer than 30 seconds.")  
* A compound sentence with a colon or em-dash separating error type from explanation

Do not apply title case or capitalize every noun. Avoid formatting that mimics UI headings or system banners unless the platform’s style requires it.
* ✅ (good) Timeout error: request took longer than 30 seconds.  
* ❌ (bad) Timeout Error: Request Took Longer Than 30 Seconds.

Punctuation should follow standard grammatical rules: if the message is a full sentence, end with a period. If it's a sentence fragment used stylistically (e.g., in micro-UIs), omit the period only if platform conventions demand it.

## Glossary and term definitions
Use sentence case when writing glossary entries and definitions, unless the term itself is a proper noun, brand name, or standard acronym. Most glossary terms are common nouns or compound nouns, and do not require capitalization unless formally registered or branded.

**Capitalize:**
* Proper nouns: names of companies, services, branded features  
    * ✅ WellnessLiving  
    * ✅ FitLIVE  
    * ❌ fitlive  
* Acronyms and initialisms: standard, fully capitalized abbreviations  
    * ✅ API  
    * ✅ JWT  

**Don't capitalize:**
* Generic technical terms  
    * ✅ webhook  
    * ❌ Webhook  
    * ✅ timeout  
* Inflected noun forms unless part of a brand  
    * ✅ access tokens  
    * ✅ webhooks

Glossary definitions typically appear in developer portals, onboarding glossaries, or field references. Ensure the term itself reflects the naming standard, and the definition remains neutral, complete, and aligned with how the term is used across product documentation.

## Links and references
Use sentence case for link text, even when referencing internal code documentation or developer tools. Link text should be treated as part of the surrounding sentence and follow conventional sentence capitalization rules.

Avoid applying title case unless the article you're referencing uses it in its title. Instead, treat the link as a noun phrase or clause-level reference embedded within your sentence, capitalizing only proper nouns and acronyms.
* ✅ For more information, consult the WellnessLiving authentication guide.  
* ❌ For more information, consult the WellnessLiving Authentication Guide.

## Acronyms and initialisms
Use ALL CAPS for standard acronyms and initialisms. By default, spell out the full term on first use, followed by the acronym in parentheses, unless the acronym is already universally recognized in developer contexts.

Capitalize all letters in initialisms, in which each letter is pronounced individually (e.g., API, JWT, HTTP), and in acronyms, which are read as words (e.g., HATEOAS, JSON).
* ✅ Hypermedia as the Engine of Application State (HATEOAS)  
* ✅ JSON  
* ❌ Json

Acronyms and initialisms like JSON, API, and HTTP do not need to be spelled out in most developer documentation because they are part of standard technical vocabulary. Writers can rely on common industry conventions and the assumed baseline knowledge of a developer audience when deciding whether to expand an acronym.