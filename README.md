# Microsoft Fabric Decision Records

This repository maintains architectural and technical decision documents for Microsoft Fabric implementations. The purpose is to document key decisions, rationale, and context for why specific approaches were chosen.

## Purpose

This repository serves as a central location for:
- Architectural Decision Records (ADRs)
- Technical decisions related to Microsoft Fabric
- Context and rationale for implementation choices
- Historical reference for decision-making processes

## Structure

```
.
├── docs/
│   ├── decisions/          # All decision documents
│   │   ├── 0001-example-decision.md
│   │   └── ...
│   ├── templates/          # Templates for new decisions
│   │   └── decision-template.md
│   └── decisions-index.md  # Index of all decisions
└── README.md
```

## How to Use

### Reading Decision Documents

All decision documents are located in the `docs/decisions/` directory. Each decision is numbered sequentially and follows a consistent format. See the [Decisions Index](docs/decisions-index.md) for a complete list.

### Creating a New Decision Document

1. Use the template at `docs/templates/decision-template.md`
2. Number the decision sequentially (find the last decision number and add 1)
3. Save it in `docs/decisions/` with format: `XXXX-brief-title.md`
4. Update the `docs/decisions-index.md` with the new decision
5. Submit a pull request with your decision document

## What is Microsoft Fabric?

Microsoft Fabric is an all-in-one analytics solution for enterprises that covers everything from data movement to data science, real-time analytics, and business intelligence. This repository documents decisions made when implementing and utilizing Microsoft Fabric.

## Contributing

When documenting a decision:
- Be clear and concise
- Include the context that led to the decision
- Document alternatives that were considered
- Explain the consequences of the decision
- Keep decisions immutable (don't edit past decisions; create new ones if changes are needed)

## License

This documentation is maintained for organizational knowledge sharing.