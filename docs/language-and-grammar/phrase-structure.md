Technical writers regularly face decisions about phrasing. The best phrasing choice depends on where the text appears and who will read it. For instance, API field names and metadata labels require compact, rigid terms that developers can quickly recognize. Tutorials, FAQs, and blog posts can afford to use longer, more natural-sounding sentences that help new readers understand complex concepts.

The style protocols below are not exhaustive, but they address critical, common choices that influence how effectively our documentation reaches a broad and diverse audience. When uncertain, aim for phrasing that's both precise enough for specialists and accessible enough for new or non-technical users.

## Labels vs. sentences
**Labels** are concise noun-based phrases (often noun-noun compounds, but sometimes single nouns) used primarily to identify UI elements, API fields, buttons, column headers, and navigation links. They must be short, scannable, and free of unnecessary words. **Sentences**, by contrast, fully explain a concept or behavior and appear in help text, tooltips, instructions, error messages, and descriptive content.

* ✅ (good label) session timeout  
    * Why good: short, clear, and immediately scannable. It succinctly names the concept without extra words.  
* ✅ (good label, single noun) duration  
    * Why good: single nouns can be effective when the context is clear and no ambiguity is introduced.  
* ❌ (bad label) the session timeout value  
    * Why bad: includes unnecessary articles ("the") and additional descriptive words ("value") that don't belong in concise labels.  
* ✅ (good sentence) "The session timeout value determines how long a client session stays active."  
    * Why good: provides context and clearly explains the meaning and behavior of the labeled item.  
* ❌ (bad sentence) "Session timeout value determine how long client session."  
    * Why bad: grammatical errors, missing words, and awkward phrasing make it hard to understand.  

### Where to use:
* Use **labels** in forms, buttons, table headings, navigation menus, and UI strings where brevity is essential.  
* Use **sentences** in instructional text, explanatory paragraphs, tooltips, and onboarding material to provide clarity and detail.

## Compactness vs. clarity
**Compact phrasing** involves stacking nouns closely together without intervening words, which saves space. **Clarity phrasing** inserts articles, prepositions, or verbs to help readers parse meaning quickly and accurately.

* ✅ (good compact) invoice batch export  
    * Why good: concise, effective for UI and lists.
* ❌ (bad compact) invoice batch export interval period  
    * Why bad: overly complex noun stacking makes meaning unclear.  
* ✅ (good clarity) "Adjust the interval for exporting the invoice batch."  
    * Why good: the added prepositions and verbs clearly define the relationship among nouns.  

#### Where to use:
* Use **compact phrases** for UI labels, settings pages, tables, dashboards, and anywhere screen space is limited.  
* Use **clarity phrasing** in longer-form explanations, introductory paragraphs, and user instructions.

## Defining vs. describing
**Defining phrases** succinctly introduce and name a concept or term. **Describing phrases** explicitly explain how that concept functions or why it matters.

* ✅ (good definition) auto-renew threshold  
    * Why good: clearly and succinctly names a concept.  
* ❌ (bad definition) threshold that automatically renews memberships  
    * Why bad: unnecessarily long for a term definition, contains verb structure better suited for a description.  
* ✅ (good description) "The auto-renew threshold determines when a membership renews automatically."  
    * Why good: clearly explains the term’s function and purpose in plain language.  

### Where to use:
* Use **definitions** in glossary entries, schema documentation, or settings. 
* Use **descriptive phrases** in explanatory content, tutorials, and user onboarding documentation.

## Naming vs. explaining
**Naming phrases** create identifiers or short names for concepts or fields. **Explaining phrases** provide context and understanding around those terms.

* ✅ (good name) client time zone
    * Why good: concise and clear, suited for identifiers and labels.
* ❌ (bad name) the time zone of the client
    * Why bad: too wordy and unsuitable as a brief identifier.  
* ✅ (good explanation) "Store the client’s time zone so appointment times render correctly."  
    * Why good: provides reasoning and clear usage context.  

### Where to use:
* Use **naming phrases** in database schemas, field names, labels, and API documentation. 
* Use **explaining phrases** in user guides, onboarding docs, and explanatory sections of documentation.

## Scannable vs. conversational
**Scannable phrasing** is brief, structured, and repetitive for quick visual recognition. **Conversational phrasing** is natural, fluid, and reader-friendly.

* ✅ (good scannable) booking lead time
    * Why good: easy to recognize in a settings menu or table.
* ❌ (bad scannable) how long before a client can book
    * Why bad: too conversational and cumbersome for quick scanning.
* ✅ (good conversational) "Specify how long before a client can book an appointment."
    * Why good: natural and approachable for first-time users.

### Where to use:
* Use **scannable phrasing** in dashboards, settings, and summary tables. 
* Use **conversational phrasing** in help center articles, tutorials, and onboarding content.

## Schema vs. prose
**Schema** documentation requires rigid, consistent phrases that align directly to database fields, JSON keys, and API parameters. **Prose** translates these rigid terms into complete, reader-friendly explanations.

* ✅ (good schema) `client_id`
    * Why good: brief, explicit, and matches precisely with database/API conventions.
* ❌ (bad schema) the identifier for a client
    * Why bad: too verbose, unsuitable for JSON keys or schema definitions.
* ✅ (good prose) "The `client_id` field uniquely identifies a client record."
    * Why good: provides context and meaning clearly for readers unfamiliar with the technical term.

!!! note
    
    For additional formatting guidelines for API fields and parameters, see the WellnessLiving API design guide.

### Where to use:
* Use **schema phrases** exclusively in schemas, code examples, API specifications, and developer guides. 
* Use **prose explanations** in explanatory paragraphs, reference articles, and guides intended for wider audiences.

## Single-word terms vs. multi-word phrases
**Single-word terms** are compact but can introduce ambiguity, whereas **multi-word phrases** specify meaning clearly.

* ❌ (bad single-word) timeout (when multiple timeout settings exist)
    * Why bad: unclear if multiple timeouts exist; too ambiguous.
* ✅ (good multi-word) session timeout
    * Why good: specific and clear, immediately distinguishes from other timeouts.

### Where to use:
* Only use **single-word terms** when the context provides clear meaning. 
* Use **multi-word phrases** for situations requiring clarity.

## Parallelism vs. variation
**Parallelism** keeps related items consistent in phrasing for easy scanning. **Variation** intentionally deviates from parallel phrasing for clarity or precision.

* ✅ (good parallel) appointment start time, appointment end time, appointment buffer
    * Why good: consistent phrasing facilitates quick visual scanning.
* ❌ (bad parallel) time before appointment starts, appointment end time
    * Why bad: inconsistent syntax slows down readers.

### Where to use:
Use **parallel structure** in lists, tables, or groups of related fields. **Vary structure** only if readability greatly improves for one particular case.

## Technical parlance vs. user empathy
**Technical parlance** uses industry terms suited for technical audiences. **User empathy** translates jargon into clear, approachable language.

* ✅ (good technical) JWT refresh token
    * Why good: precise, standard technical jargon suitable for developers.
* ❌ (bad technical for users) renew auth token
    * Why bad: unnecessarily abbreviated and cryptic for end-users.
* ✅ (good empathetic) "Your authentication token renews automatically when it expires."
    * Why good: friendly and approachable wording helps users understand.

### Where to use:
Use **technical jargon** in engineering docs, API references, and developer content. Use **empathetic language** in customer-facing tutorials, user guides, and support content.

## Consistency vs. local clarity
**Consistency** keeps terminology uniform across screens and teams. **Local clarity** allows alternative terms when they significantly aid user understanding.

* ✅ (good consistent) user profile image across all UIs
    * Why good: predictable phrasing reduces cognitive load.
* ❌ (bad consistent) mixing avatar and profile photo
    * Why bad: inconsistent terminology confuses users.
* ✅ (good local clarity) "The profile photo (also called an avatar) is visible to other clients."
    * Why good: introduces alternate terminology explicitly without sacrificing overall consistency.

### Where to use:
Default to **consistent terms** across documentation. Only introduce **alternative terminology** explicitly where necessary for immediate user comprehension.