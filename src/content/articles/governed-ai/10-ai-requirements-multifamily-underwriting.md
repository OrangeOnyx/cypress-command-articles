---
title: "AI Requirements for Multifamily Underwriting"
series: "The Governed AI Series"
part: "Part I — Draw the Boundary"
eyebrow: "DRAW THE BOUNDARY"
deck: "Apartment underwriting is a pool of short leases, not a stack of retail tenants. What a model may extract from the rent roll and the T12, how loss-to-lease is sourced, and who signs the NOI."
author: "Cypress Command"
date: "2026-09-28"
read_time: "16 min"
desk: "buy"
status: "review"
source: "batch-e"
---

# AI Requirements for Multifamily Underwriting

Multifamily underwriting does not work like a shopping center. In retail, one tenant can be the deal. In an apartment property, no single resident is material. What matters is the pool: vacancy, collections, concessions, turnover, and how far in-place rents sit from a market rent you can defend. Agency lenders, life companies, conduits, and debt funds all ask for that pool in a precise form. A model can build the tables. It cannot choose the market rent or sign the debt service coverage.

This article is the boundary for that work. Figures are synthetic. They are not a named community and not a loan quote. The file the outputs have to live in is "AI Requirements for CRE Underwriting: A Complete Governance Guide." Sponsor cash flow is "Sponsor Financial Spreading with AI," not a paragraph at the end of the rent roll.

## The unit of analysis

A shopping-center file is lease by lease. A multifamily file is unit by unit, then rolled up. The three documents that carry the roll-up are the rent roll, the trailing twelve-month operating statement, and a market-rent source that is not the owner's column on the rent roll. From those, a person can support a net operating income. A model can draft the support.

| Subtype | How the roll is usually counted | A risk the model should surface, not decide |
|---|---|---|
| Garden | Units, often 12-month leases | Turnover cost and thin maintenance |
| Mid-rise or high-rise | Units, concessions, loss-to-lease | Owner "market rent" above the comps |
| Build-to-rent | Homes, sometimes longer leases | Lease-up pace versus the pro forma |
| Student | Beds, an academic calendar | Enrollment and a parent guaranty |
| Senior | Units or beds, short stays | Operator quality and census, plus regulatory questions for counsel |

Assets are the building, the unit mix, and the condition. Operations are collections, staffing, and the quality of NOI. Risk is vacancy, coverage, the sponsor, and the citations. That is the same three-part frame as "Assets, operations, risk," aimed at a different asset.

## The rent roll

The roll is a snapshot: unit, type, area, resident, lease dates, contract rent, concessions, notice, and whether the unit is vacant, a model, or down. Rolls arrive as workbook exports, PDF prints, and scans. The model's first job is one schema. Its second job is to refuse a field it cannot read.

Extract, then check:

| Field | Check | A flag, not a verdict |
|---|---|---|
| Contract rent | Against T12 collections | Roll potential far above collections |
| Expiration | A 12- to 24-month schedule | A large share expiring inside 90 days |
| Vacancy | Physical versus economic | The roll looks full and the cash does not |
| Concessions | Free months and discounted rent | Concessions on the roll and missing from the T12 |
| Unit count | Against the appraisal or survey | A count that does not match |
| Owner's market-rent column | Against a third-party survey | Owner rents well above the comps |

A lease-expiration schedule is the retail rollover schedule in miniature. A property with a large share of leases ending inside one quarter has turnover risk even if today's occupancy is high. The model can count the expirations. The underwriter decides whether the leasing team can absorb them.

Cross-read the roll and the T12. If the roll says 95 percent occupied and collected rent looks like 88 percent, stop. The gap may be bad debt, residents still listed who are not paying, or a roll cleaned up for the sale. That cross-read is worth more than a faster cap-rate math.

## Income, from potential to effective

The waterfall is ordinary. The discipline is naming which rent the potential uses.

- **Gross potential rent.** Every unit at the rent you chose, for twelve months. Owners often use in-place rent and call it potential. That hides loss-to-lease. The model should say which column it used.
- **Loss-to-lease.** Potential at market minus in-place contract rent. Below.
- **Physical vacancy.** Empty units.
- **Bad debt and concessions.** Uncollected rent and free rent.
- **Other income.** Application fees, late fees, pets, parking, laundry, storage, utility reimbursements.
- **Effective gross income.** The income the expense ratio and the loan will sit on.

Other income is easy to under-count because it is scattered. Illustrative only: 200 units at $50 a unit a month is $120,000 a year. That is a teaching product, not a market study. Normalize other income per unit and compare it with the story in the offering memo. Flags a reviewer should see: potential built on in-place rents; vacancy under 5 percent on a property you are calling stabilized, with no explanation; bad debt under 1 percent with no support; concessions on the roll that never hit the T12; other income that jumps more than about 20 percent month to month; utility reimbursement that does not match the billing method in the documents.

## Expenses the owner did not charge

Owner T12s understate the cost of a third-party operation. The usual holes are the management fee, payroll, maintenance, and a capital reserve. The model maps lines to a schema and benchmarks per unit only against figures you supply or mark as a screen.

| Category | Owner pitfall | What the file does | A teaching screen, not a bid |
|---|---|---|---|
| Management fee | Zero, because the owner self-manages | Insert a stated percent of EGI | Often 4–6 percent institutional, 6–8 percent smaller assets |
| Repairs | Deferred, so the line looks efficient | Compare per unit and ask | Often discussed around $600–$1,200 per unit per year |
| Payroll | Missing | Add the staffing you will actually carry | Often discussed around $800–$1,500 per unit per year |
| Insurance | Buried in a portfolio policy | Price the policy you will buy | Often discussed around $300–$600 per unit per year |
| Taxes | Pre-sale assessment | Model the reassessment rule that applies | Local, from the bill and the statute |
| Common-area utilities | Partial months | Annualize and cite | Often discussed around $200–$500 per unit per year |
| Capital reserve | Absent | Add the reserve the lender or buyer will use | Often discussed around $250–$400 per unit per year |
| Administrative | Personal costs in the property | Remove what is not the property | Often discussed around $150–$300 per unit per year |

Illustrative management-fee hole: a 150-unit property, self-managed, no fee line. If effective gross income supports a 4 to 6 percent fee in a band of roughly $60,000 to $90,000, the owner's NOI is high by that amount. The model flags the blank line. The person writes the percent and cites it. Do not underwrite the unadjusted NOI.

## Loss-to-lease needs a market rent you did not get from the seller

Loss-to-lease is market potential minus in-place contract rent on occupied units. It is the upside story and the risk story at once. As leases roll, rent can move toward the market. If the market was overstated, the upside was never there.

Steps:

1. Take market rent by unit type from a third-party survey or an appraisal, not from the owner's column.
2. Potential equals unit count times that rent times twelve, summed across types.
3. In-place equals contract rent from the roll, annualized.
4. Loss-to-lease equals potential minus in-place.
5. The ratio is loss-to-lease divided by potential.

Teaching property, 120 units, no real name:

| Type | Count | Market rent / month | In-place average |
|---|---|---|---|
| One-bedroom | 80 | $1,150 | $1,050 |
| Two-bedroom | 40 | $1,450 | $1,280 |

Potential is (80 × 1,150 + 40 × 1,450) × 12 = $1,800,000. In-place is (80 × 1,050 + 40 × 1,280) × 12 = $1,622,400. Loss-to-lease is $177,600, about 9.9 percent of potential. A screen practitioners use: under 5 percent looks stabilized, 5 to 10 percent is modest upside, 10 to 20 percent is a value-add case that needs a lease-by-lease timing, above that the market rent itself is the thing to audit. The 9.9 percent result is only as good as the $1,150 and $1,450. If those came from the owner and sit more than about 5 to 10 percent over the comps, the model flags the source and the upside waits.

## Sponsor, briefly

Agency files ask for a personal financial statement, returns, a schedule of real estate owned, and liquidity. A common agency screen, confirm with the lender, is net worth on the order of the loan and post-closing liquidity on the order of 10 percent of the loan. The model can extract. It must not skip a property on the schedule. Global cash flow that ignores the rest of the portfolio is not global. The method is the sponsor article. Do not duplicate a thin version here and call it done.

## The workflow and the gate

Order matters. Completeness, then extraction, then the income waterfall, then expenses, then loss-to-lease from an outside rent source, then the sponsor spread, then scenarios a person defined, then a signature.

A staffing comparison, illustrative, not a measured Cypress Command result: a 200-unit package might take an analyst most of one to two days by hand, and the extraction pass might come back in well under an hour, with one to two hours of review. The review is the product. Time saved that skips the review is a faster error.

Five file rules:

1. Every extracted value cites a document, page, and line.
2. Every normalization states the rule and the rate the person chose.
3. A named underwriter signs before the number enters the credit model.
4. The output is versioned. A silent edit is a new version.
5. A low-confidence or unreadable field is re-read, not averaged.

### The view from Arnould Blvd

On The Blvd is retail: 101–149 Arnould Blvd, Lafayette, roughly 63,000 square feet, 27 units, two buildings, Command Platform as the lease record. It is not an apartment community, and this article does not apply a unit-mix waterfall to it. The plate is the contrast. There, one lease can move the income. Here, no resident does, and the market-rent column is the place a story gets inflated. The signature rule does not change with the asset. The owner, or the underwriter the owner named, signs. The model does not.

## The practical next step

1. List the rent roll, the T12, and the market-rent source as three separate documents. If the third is the owner's column, say so and do not book the upside.
2. Count leases expiring in the next 90 days. Write the share of units, not a vibe.
3. Find the management-fee line. If it is blank, the NOI is not finished.
4. Build the five-line loss-to-lease math for one unit type before you automate the property.
5. Point the sponsor documents at the sponsor article, and point the signed NOI at the governance guide.

---

*Cypress Command builds practical AI-enabled operating systems for owner-led businesses — including the owners and operators of commercial real estate. This article is educational. It is not legal, tax, or investment advice.*
