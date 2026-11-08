# Kervra

**Strength, built daily.**

Kervra is intended to be free to use and open-source: a fitness and wellness application planned for Android and iOS, built with Flutter and Dart. It is intended for people who want a calm, practical place to understand and record their training, nutrition, hydration, activity, recovery, and progress.

- **Repository:** [github.com/Avnish-Alves/kervra](https://github.com/Avnish-Alves/kervra)
- **Maintainer:** Avnish Alves

## Philosophy and vision

Kervra is being designed around consistent habits, personal agency, and respect for the user's data. It should support a range of experience levels without shame, pressure, or diagnostic claims. The long-term vision is a useful, accessible companion that helps people see their own patterns and make informed choices.

## Planned V1 capabilities

The V1 scope is planned to include:

- A dashboard for a concise view of current activity and goals.
- Training and workout logging.
- Nutrition and meal logging.
- Hydration tracking.
- Progress views that preserve historical records.
- Recovery and general activity tracking.
- Read-only health integrations. Their implementation depends on platform capabilities, technical validation, and user consent.

These are planned capabilities; they are not represented as implemented features.

## Local-first operation

Kervra is intended to work offline and keep the user's records on their device by default. Core use should not require an account or backend. Any future platform integrations should be optional, read-only where specified, and explicit about data access. Export and restore are planned so people can retain control of their records. Implementation and security details remain under development.

## Development status

**Pre-alpha — under active development.** The repository is currently at its documentation foundation. The Flutter application, setup workflow, and V1 capabilities are not yet implemented, so there are no setup commands to provide accurately.

## Roadmap

### Planned

- Establish the app foundation and architecture.
- Build the V1 capabilities listed above, with accessible light and dark themes.
- Define and implement local data ownership, export, and restoration.

### Deferred

- Optional cloud sync or multi-device features, pending privacy and architecture decisions.
- Write access to health platforms, pending separate product and safety review.

### Excluded from the current product direction

- Mandatory accounts or a required backend.
- Diagnostic or medical claims.
- Shame-based messaging or punitive streaks.

Roadmap items may change as the project develops; no release dates are established.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md), [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md), and [SECURITY.md](SECURITY.md) for contribution guidance. Community contributions are not being accepted until a reporting contact is configured in the Code of Conduct. Contributions should preserve privacy, offline operation, accessibility, and maintainability.

## License

Kervra is offered under the Apache License 2.0. See [LICENSE](LICENSE).
