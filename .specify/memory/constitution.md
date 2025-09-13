# MusicShift Constitution

## Core Principles

### Frontend Architecture
- **Framework**: Angular
- **UI Components**: Angular Material with a custom theme.
- **Styling**: SCSS and CSS. Tailwind CSS is not to be used.
- **Structure**: Code should be organized into `packages` (instead of `libs`).

### Backend Architecture
- **Framework**: NestJS monolith.
- **Database**: PostgreSQL with Mikro-ORM.
- **Pattern**: Clean Architecture.
- **Structure**: Code should be organized into `packages` (libraries).

### General
- **Testing**: TDD is mandatory. Tests must be written before implementation.
- **Integration Testing**: Required for new library contracts, contract changes, and inter-service communication.

## Governance
- This constitution supersedes all other practices.
- All pull requests and reviews must verify compliance with this constitution.

**Version**: 1.0.0 | **Ratified**: 2025-09-12 | **Last Amended**: 2025-09-12
