Treat your OpenAPI (Swagger) definitions as the single source of truth. Every endpoint, model and error response should be defined in a machine-readable spec, then used to generate client SDKs, mock servers and code samples.

Key developer actions:

* Maintain a complete OpenAPI 3.0+ spec and update it alongside any API change.
* Generate and publish client libraries (e.g., Python, TypeScript, PHP) automatically from that spec.
* Use spec-driven tests in CI/CD to check for contract drift.
* Include example payloads and response schemas.
* Use semantic versioning (e.g., v2.5.0) and tag Git releases accordingly.