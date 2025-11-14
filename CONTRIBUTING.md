# Contributing to Microsoft Fabric Decision Records

Thank you for contributing to our decision documentation! This guide will help you understand how to create and submit decision documents.

## When to Create a Decision Document

Create a decision document when:

- Making an architectural choice that affects the overall system design
- Selecting a technology, tool, or framework for the project
- Choosing a specific Microsoft Fabric feature or approach
- Making a decision that has long-term implications
- Selecting between multiple viable alternatives
- Making a trade-off that future team members should understand

**Don't create a decision document for:**
- Minor implementation details
- Obvious or standard practices
- Temporary workarounds
- Day-to-day tactical decisions

## How to Create a Decision Document

### Step 1: Determine the Decision Number

Find the highest numbered decision in `docs/decisions/` and add 1. Use 4-digit zero-padding (e.g., 0001, 0002, 0003).

```bash
# List existing decisions
ls docs/decisions/

# If the last one is 0001, your new decision will be 0002
```

### Step 2: Copy the Template

```bash
cp docs/templates/decision-template.md docs/decisions/XXXX-your-brief-title.md
```

Replace `XXXX` with your decision number and `your-brief-title` with a short, descriptive title using kebab-case.

### Step 3: Fill in the Template

Complete all sections of the template:

- **Title**: Clear, concise title (50 characters or less)
- **Date**: Use YYYY-MM-DD format
- **Status**: Usually starts as "Proposed", changes to "Accepted" when merged
- **Context**: Explain the background and why this decision is needed
- **Decision**: State clearly what was decided
- **Alternatives Considered**: List and explain why other options were rejected
- **Consequences**: Document both positive and negative outcomes
- **Implementation Notes**: Any specific details about implementation
- **References**: Links to relevant documentation or resources

### Step 4: Update the Index

Add your decision to the table in `docs/decisions-index.md`:

```markdown
| [XXXX](decisions/XXXX-your-brief-title.md) | Your Title | YYYY-MM-DD | Proposed |
```

### Step 5: Submit a Pull Request

1. Commit your changes with a clear message:
   ```bash
   git add docs/decisions/XXXX-*.md docs/decisions-index.md
   git commit -m "Add decision XXXX: Your Brief Title"
   ```

2. Push your branch and create a pull request

3. Request review from relevant stakeholders

### Step 6: Update Status

Once the PR is approved and merged, the status should be changed from "Proposed" to "Accepted" (this can be done during the PR review process).

## Decision Lifecycle

1. **Proposed**: Initial state when decision is submitted for review
2. **Accepted**: Decision has been approved and merged
3. **Deprecated**: Decision is no longer relevant (add note explaining why)
4. **Superseded**: Decision has been replaced by a newer decision (link to the new one)

## Guidelines for Good Decision Documents

### Be Clear and Concise

- Use simple language
- Avoid jargon unless necessary
- Get to the point quickly

### Provide Context

- Explain the problem you're solving
- Describe the current state
- Identify constraints and requirements

### Document Alternatives

- Show you've considered other options
- Explain why alternatives weren't chosen
- Be fair in your assessment

### Be Honest About Trade-offs

- Every decision has pros and cons
- Document both positive and negative consequences
- Don't oversell your decision

### Make It Permanent

- Once accepted, decisions are immutable
- If circumstances change, create a new decision that supersedes the old one
- This preserves historical context

## Example Decision Document

See [0001-use-adr-for-decision-tracking.md](docs/decisions/0001-use-adr-for-decision-tracking.md) for a complete example of a well-written decision document.

## Questions?

If you have questions about the decision documentation process, please:
- Review existing decision documents for examples
- Check the [README.md](README.md) for an overview
- Ask in your team chat or during team meetings

## Microsoft Fabric Specific Considerations

When documenting Microsoft Fabric decisions, consider including:

- Which Fabric workload(s) are affected (Data Factory, Synapse, Power BI, etc.)
- Performance implications
- Cost considerations
- Scalability factors
- Security and compliance aspects
- Integration with other Fabric or Azure services

Thank you for helping maintain high-quality decision documentation!
