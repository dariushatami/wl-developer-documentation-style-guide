Tense choice is a key factor in readability. Default to simple present because it expresses general truths and habitual actions, which is the standard for describing software functions.

Simple present: Use for describing stable system behavior, commands, and ongoing truths.
✅ (good) The `auth.generate_token()` method returns a token object.

Simple future: Use only when describing an inevitable future action following a condition.
✅ (good) If the key is invalid, the API will return a 401 error.

Simple past: Use to describe discrete, completed events (e.g., changelogs, bug reports, and historical notes).
✅ (good) The 2.1 release introduced the new reporting API.

Avoid unnecessary tense shifts within the same context. Keep instructions in present tense even if the user will execute them later.