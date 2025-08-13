Notes and warnings draw attention to information that would be overlooked in normal flow but is critical for successful implementation or safe system use. Use them sparingly to avoid diluting their impact.

## Notes
Use a note to highlight important but non-destructive information. Common cases include:
* API limitations, such as maximum request size  
* Feature availability, such as enterprise-only capabilities  
* Contextual tips for a specific workflow  

## Warnings
Use a warning to draw attention to conditions that can cause:
* Data loss  
* Service interruption  
* Irreversible changes  

!!! note "Publishing platform features"
    This note itself is an example of an MkDocs Material **note admonition**. In developer documentation, notes and warnings are often rendered through platform features that provide consistent visual styling and accessibility.  

    Examples of platform implementations include:  
    - **MkDocs with Material**: `!!! note` and `!!! warning` admonitions  
    - **Docusaurus**: `<Admonition type="note">` components  
    - **Sphinx**: `.. note::` directives in reStructuredText  
    - **Jupyter Book**: `{note}` and `{warning}` MyST Markdown blocks  

    Using the platform’s built-in notes feature ensures that important information is visually distinct, easily scannable, and consistently styled across all documentation.
