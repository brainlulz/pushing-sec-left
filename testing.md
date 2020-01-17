# Testing

Happens in Coding, Testing and Release/Maintenance.

Feedback as soon as possible.

Prodive devs security scanning software (ZAP). Fix before sending to QA.

Add automated testing into pipeline:

- VA scanning of infrastructure
- 3rd party components and libraries
- Dynamic Application Security Testing (passive scan)
- SAST can be slow
- Security hygiene: encryption status, headers, HTTPS...
- repurpose unit tests into regressive sec tests
- For each test create an opposite test
- Create a unit test to ensure the bug doesn't reappear
- Pass tests before pushing to the pipeline
