# CapitalLens

**AI-assisted investment assumption reconciliation for analysts and investment committees**

**Status:** Selected for presentation at the 2026 Investment Management for All: Wealth & Women AI Showcase at UNC Kenan-Flagler Business School

[Back to project portfolio](../../README.md)

## Project overview

CapitalLens is a proposed quality-control tool for investment research. It compares the assumptions in an analyst's financial model and investment memo with the latest source evidence, identifies discrepancies, and prepares a traceable review package before an investment committee meeting.

Investment recommendations are assembled from materials that change at different times: models, filings, earnings calls, debt documents, market data, internal notes, and draft memos. A model may retain old guidance, a memo may use a different definition of free cash flow, or an exit assumption may no longer match comparable-company valuations. CapitalLens is designed to make that reconciliation process more systematic, repeatable, and auditable.

## Proposed workflow

1. **Read the working file set.** Connect the model, memo, filings, transcripts, debt documents, and approved market evidence while recording document dates and versions.
2. **Build an assumption ledger.** Extract material values and claims, including revenue growth, margins, capital expenditures, leverage, refinancing costs, valuation multiples, and management guidance. Retain the source and exact location for each entry.
3. **Reconcile the evidence.** Compare equivalent assumptions across files and test whether their values, periods, units, definitions, and dates agree.
4. **Assess the investment impact.** Explain how a discrepancy may affect valuation, debt-service capacity, covenant headroom, private-equity returns, or private-credit downside protection.
5. **Prepare the review package.** Produce a ranked discrepancy report, questions for management or the deal team, model inputs requiring review, and a source-linked appendix.

## Illustrative output

The values below are hypothetical and demonstrate the form of the review.

| Assumption | Model or memo | Latest evidence | Finding | Possible effect |
| --- | ---: | --- | --- | --- |
| 2027 revenue growth | 6.0% | Management guidance implies 3% to 4% | Conflict | Valuation and debt-service capacity |
| Exit multiple | 12.0x | Selected public comparables trade near 8.5x | Unsupported | Private-equity return may be overstated |
| Annual debt repayment | $75 million | Planned capital spending reduces available cash | Conflict | Deleveraging may take longer |
| Refinancing rate | 5.5% | Comparable debt yields are 7.2% | Stale | Interest expense may be understated |

## Why it is different from a chat prompt

The language model would be one component of CapitalLens. The product value comes from the controlled system around it:

- Direct model-to-source comparison
- A persistent assumption ledger
- Document and model version tracking
- Standardized materiality rules
- Source-linked findings
- Repeatable review when new information arrives
- Preservation of unresolved conflicts for human review

A general-purpose AI assistant can perform parts of the task when an analyst selects the right files and writes the right prompts. CapitalLens is intended to run the same structured process across a team's working files and preserve the results for review.

## Pilot and validation plan

The initial prototype will use the IM4A Fundamental Investing case. It will extract assumptions from a case memo and simple model, link them to the provided source packet, and generate a discrepancy report.

The demonstration will update one source or model input and show how the assumption ledger, affected conclusions, and review questions change. The pilot will compare CapitalLens with a manual review using two measures:

- Time required for the first reconciliation pass
- Number of material discrepancies identified

## Controls and limitations

CapitalLens is intended to support investment judgment, not replace it. The proposed controls include approved-source restrictions, citations for material flags, separation of facts from analyst assumptions, preservation of unresolved conflicts, and human confirmation before any model or memo changes.

## My contribution

I developed the problem definition, product concept, workflow, validation plan, sample output, and investment-use cases. The project is currently moving from concept design toward a showcase-ready prototype and demonstration.

## Next steps

- Design the assumption-ledger data structure
- Build a small working prototype using the Fundamental Investing case
- Test model-to-source comparison and version updates
- Document failure cases and human-review controls
- Prepare the final showcase PDF and two-to-three-minute demonstration
