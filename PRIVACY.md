# Privacy

## Intended model

Kervra's design goal is to be local-first and offline-first. The intended model is for personal fitness and wellness records to remain on the user's device by default, with core functionality requiring no account or backend. Users should retain control over whether any future optional integrations can read data. These are intended principles, not implemented behavior or guarantees.

## Current implementation

The repository is at its documentation foundation. There is no application implementation yet, so no data collection, storage behavior, integrations, encryption, backup, or other security controls are currently provided by Kervra.

## Planned behavior

The product plan is for training, nutrition, hydration, activity, recovery, and progress records to be stored locally. Read-only health integrations are planned for consideration; they are not implemented. Their feasibility, permissions, data scope, platform behavior, and any data retention will require technical validation, explicit design, and user consent.

Export and restoration are intended product capabilities so users can preserve and move their records; neither is implemented. Encryption and backup are not implemented, and their design remains unresolved. Synchronization is not implemented and is not part of the initial direction; any later consideration would require separate privacy and architecture review. No integrations currently exist.

## Health information

Kervra is a fitness and wellness tool, not a diagnostic service. Users should not treat it as medical advice. The project will need to document actual data flows and platform permissions before release; this document describes intended principles, not a guarantee about an implementation that does not yet exist.
