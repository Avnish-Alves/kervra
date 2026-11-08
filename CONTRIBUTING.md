# Contributing to Kervra

Kervra is pre-alpha and under active development. The project repository is [github.com/Avnish-Alves/kervra](https://github.com/Avnish-Alves/kervra), maintained by Avnish Alves. Community contributions are not being accepted until a confirmed reporting contact is configured in the [Code of Conduct](CODE_OF_CONDUCT.md).

## Before starting

- Check existing issues and discussions for related work.
- For substantial changes, open an issue to discuss the problem and approach before implementation.
- Keep proposals aligned with user privacy, local-first and offline-first operation, accessibility, and the product scope.

## Issues and pull requests

Use GitHub issues to report reproducible problems or propose changes. Include relevant context and steps to reproduce without sharing private health or personal data. Pull requests should explain the problem, summarize the change, link a related issue where applicable, and note any user-visible or data-format impact. Keep changes focused and update relevant documentation. Do not include secrets or real personal health records in examples, fixtures, or screenshots.

## Coding standards

When application code is introduced, use idiomatic null-safe Dart and established Flutter conventions. Prefer small, maintainable, independently testable changes; handle loading, empty, success, and error states; support accessibility and light and dark themes; and avoid unnecessary dependencies. Follow the architecture and formatting choices adopted by the project at that time. Do not introduce product or architecture decisions silently.

## Tests and documentation

Add or update tests for meaningful behavior and run relevant analysis and tests for code changes. Report commands and results accurately, including failures. Update documentation when behavior, setup, data handling, or user-facing decisions change. Do not claim unrun checks have passed.

## Privacy and local-first requirements

Contributions must not undermine local-first and offline-first use, introduce mandatory accounts or backend services, or collect or transmit user data without explicit product and privacy review. Explain data flows and permissions for any proposed integration. Preserve historical records and user control of their data.

No DCO or CLA requirement is currently stated by this project.
