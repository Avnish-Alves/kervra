# Proposed Architecture

> This document describes proposals for discussion. None of the application architecture below is implemented or formally approved.

## Application shape

The proposed application is a Flutter modular monolith written in Dart, targeting Android and iOS. Feature-first organization would keep each product area's presentation, application logic, and data access together while allowing shared domain concepts and infrastructure to remain explicit. This avoids committing to a distributed or plugin-based architecture before there is a demonstrated need.

Proposed feature areas include dashboard, training, nutrition, hydration, progress, recovery/activity, and platform integrations. Shared concerns may include navigation, design system, persistence, and export/restore.

## Proposed technology choices

- **SQLite with Drift** for local relational persistence and typed queries.
- **Riverpod** for state management and dependency composition.
- **GoRouter** for declarative navigation.

These are candidate choices pending formal architecture approval and a review of current Flutter and platform constraints. They are not dependencies in the repository today.

## Data ownership and history

**Proposed design requirements:** The user should own records stored locally on their device, and core workflows should function offline without an account or backend. Data access should be limited to the feature and infrastructure layers that need it. Health platform integrations may be considered as optional, read-only sources behind explicit user permissions; imported data should remain distinguishable from user-entered data where useful. These are proposals, not implemented controls.

**Proposed design requirements:** Historical workout and nutrition records should be preserved. Where records depend on mutable reference data (for example, a food definition or training plan), the design should determine which values need snapshots so past records remain interpretable after reference data changes. Corrections and deletions should have explicit semantics rather than silently rewriting history.

## Migrations

**Proposed design requirements:** Schema changes should use versioned, tested database migrations. Migration behavior should preserve user data and handle interrupted or failed upgrades safely. The migration framework and recovery strategy remain to be selected and validated once persistence is introduced.

## Export and restore

Export and restore are planned user capabilities, not implemented features. **Proposed design requirements:** A format should be documented, versioned, and portable, with validation before restore and clear handling of conflicts or duplicates. Export should make the user's records understandable outside the app. Encryption, password protection, and backup storage are unresolved; no such protection is currently implemented or promised.

## Platform integrations

Integrations with Android and iOS health platforms are planned as optional, read-only capabilities, subject to platform capabilities, technical validation, and user consent. **Proposed design requirements:** They should request only necessary permissions, explain the data scope, tolerate unavailable permissions and platform APIs, and avoid making core app use dependent on integration access. The specific platforms, supported data types, refresh behavior, attribution/provenance, and retention rules remain undecided.

## Unresolved decisions

- Approve or replace SQLite/Drift, Riverpod, and GoRouter after a prototype and dependency review.
- Define feature boundaries, shared domain model, and dependency direction.
- Choose identifier, timestamp, unit, timezone, and localization conventions.
- Define snapshot and correction semantics for historical records.
- Specify export format, restore conflict handling, and backup protection.
- Decide how migrations recover from failure and how compatibility is tested.
- Select health integration APIs and define consent, provenance, refresh, and deletion behavior.
- Determine storage encryption requirements based on platform protections and threat review.
- Establish test coverage expectations and support for accessibility and themes across shared widgets.
