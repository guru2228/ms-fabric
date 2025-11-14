# Decision Records Index

This document provides an index of all architectural and technical decisions made for Microsoft Fabric implementations.

## Active Decisions

| Number | Title | Date | Status |
|--------|-------|------|--------|
| [0001](decisions/0001-use-adr-for-decision-tracking.md) | Use Architecture Decision Records for Decision Tracking | 2025-11-14 | Accepted |

## Deprecated Decisions

_No deprecated decisions yet._

## How to Add a New Decision

1. Copy the template from `templates/decision-template.md`
2. Create a new file in `decisions/` directory with the format `XXXX-brief-title.md` where XXXX is the next sequential number (zero-padded to 4 digits)
3. Fill in the template with your decision details
4. Add an entry to this index in the "Active Decisions" table
5. Submit a pull request

## Decision Categories

Decisions can be tagged with categories to help with organization:

- **Architecture**: Overall system architecture decisions
- **Data**: Data modeling, storage, and processing decisions
- **Integration**: Integration patterns and approaches
- **Security**: Security and compliance decisions
- **Performance**: Performance optimization decisions
- **Operations**: Operational and deployment decisions

## Notes

- Decisions are immutable once accepted. If a decision needs to change, create a new decision that supersedes the old one.
- Always provide context and rationale for decisions.
- Consider and document alternatives that were evaluated.
