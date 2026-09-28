---
title: "AI Requirements for CRE Underwriting: Shopping Centers and Owner Financials"
series: "The Shopping Center Operator Series"
part: "Part X — AI & Operating Systems"
eyebrow: "AI & OPERATING SYSTEMS"
deck: "What a model may extract from a shopping-center file, which retail clauses it has to be aimed at, and the citations a person checks before anyone calls the result underwriting."
author: "Cypress Command"
date: "2026-09-28"
read_time: "16 min"
desk: "buy"
lanes: ["governed-ai"]
status: "review"
source: "batch-e"
---

# AI Requirements for CRE Underwriting: Shopping Centers and Owner Financials

A shopping center is not a single rent. It is a stack of leases whose sales, expirations, and co-tenancy clauses move together. A model is useful on that stack because it can read faster than an analyst. It is dangerous on that stack for the same reason: a tidy rent roll looks like the whole file. This article is the operator's list of what the model may prepare, what it has to be pointed at, and what a person still signs. Figures below are synthetic. They are not On The Blvd and not a listing.

The governance file these outputs have to land in is "AI Requirements for CRE Underwriting: A Complete Governance Guide." The shorter boundary, for any business, is "AI in CRE Underwriting: What the Model Prepares and What the Owner Signs."

## Assets, operations, and risk

The field note "Assets, operations, risk" is the weekly frame. Applied to an acquisition file, it is also a way to brief a model without pretending the model owns the decision.

| Pillar | The question | What the model may prepare | What the person signs |
|---|---|---|---|
| Assets | What is being bought? | Lease abstracts, a tenant table, occupancy-cost math from sales someone supplied | The property, the constraints, and the price |
| Operations | How does income actually arrive? | A normalized T12, a chart-of-accounts map, a list of odd lines | The stabilized NOI and every adjustment |
| Risk | What protects the file? | Citation gaps, missing exhibits, scenario tables from assumptions the analyst wrote | The credit or investment decision |

A model does not supply rent growth, vacancy, or an exit cap. It can lay out a range it was given. "The model chose 3 percent" is not an assumption. It is a missing owner.

## What the model should read in the rent roll

A general pro forma blends the center into one income line. The useful pass is tenant by tenant. Point the extraction at these fields, and name the document each one comes from.

| Data point | Source | Why it is in the file |
|---|---|---|
| Base rent and area | Rent roll and lease | The start of NOI |
| Recoveries | Lease exhibits | What the landlord still pays |
| Expiration | Lease and rent roll | Rollover, not a blended occupancy rate |
| Options and steps | Lease | A below-market option is a future NOI cap |
| Co-tenancy | Lease, often an exhibit | Rent can fall if an anchor goes dark |
| Percentage rent | Lease | Upside only if sales clear a breakpoint |
| Tenant sales | Sales reports, if you have them | Occupancy cost and renewal risk |
| Guaranty | Guaranty agreement | Secondary support for a small tenant |

Incomplete packets are the ordinary failure. If the exhibits are missing, the abstract should say "exhibits not provided," not invent a recovery structure.

## Co-tenancy and percentage rent

Two clauses are where a blended model goes quiet.

A co-tenancy clause can let an inline tenant cut rent, switch to a percentage of sales, or leave if an anchor or a stated share of the center goes dark. The rent roll will not show it. A worked shape, illustrative only: an anchor suite of 40,000 square feet goes dark, and twelve inline leases allow a 50 percent rent reduction. The model can add those twelve rents and halve them. The person decides whether the trigger is real, whether notice was drafted correctly, and whether the anchor's own lease changes the story. The dollar figure is an exposure, not a conclusion.

Percentage rent is the other direction. Illustrative tenant, not a real suite:

| Variable | Value | Source |
|---|---|---|
| Area | 3,000 SF | Rent roll |
| Base rent | $30.00/SF, $90,000 a year | Lease |
| CAM, tax, and insurance | $12.00/SF, $36,000 a year | Lease exhibits |
| Total occupancy cost | $126,000 | Calculated |
| Reported sales | $700,000 | Sales report |
| Occupancy cost ratio | 18 percent ($126,000 ÷ $700,000) | Calculated |
| Percentage rent rate | 6 percent above the breakpoint | Lease |
| Natural breakpoint | $1,500,000 ($90,000 ÷ 0.06) | Calculated |
| Percentage rent due | $0, sales are below the breakpoint | Calculated |

Eighteen percent occupancy cost is a watch point in this teaching file, not a universal law. Category matters. A grocer and a jeweler do not share a healthy band. The model can rank tenants. The owner decides which ranks are real.

Where sales exist, occupancy cost is total occupancy cost divided by annual gross sales. Bands used as a screen, not as a covenant: at or under 8 percent often reads as comfortable, 10 to 14 percent as a watch, and 18 percent and above as stressed. Sales per square foot is the pair to that ratio. In the example, $700,000 on 3,000 square feet is about $233 a square foot. Both numbers go on the watch list. Neither is a renewal decision.

## Owner financials are document work

Ratio work is the last step. The slow step is reconciliation. Owner T12s do not share a chart of accounts. Management fees are often missing. Capital items sit in repairs. A termination fee inflates income. The model can apply a written rule the same way every time. It cannot decide that the rule is the right one for this property.

| Adjustment | What to look for | Effect if ignored | Treatment in the file |
|---|---|---|---|
| Management fee | No fee, or a fee under a market band | NOI too high | Normalize; a retail screen often used is 4–6 percent of effective gross income |
| Capital items in repairs | Roof, parking, major HVAC | NOI too low | Move to capital; replace with a reserve the owner chooses |
| Owner items | Personal auto, family payroll, unrelated fees | Expenses distorted | Add back only with an invoice or a tax-return tie |
| Thin repairs on an old building | A repairs line that does not match the age of the asset | NOI too high | Ask; do not let the model "correct" it silently |
| One-time income | Termination fees, insurance proceeds, grants | NOI too high | Remove from stabilized NOI and disclose |
| Vacancy | No allowance, or a rate far under the market | NOI too high | Apply a stated rate; 5–10 percent is a retail screen, not a fact about this center |
| Recoveries | CAM and tax lines that do not match the leases | Expense recovery wrong | Tie to the lease, not to the seller's label |

"How to Normalize a T12 Statement for CRE Underwriting" is the line-by-line version, with a full illustrative bridge. Sponsor and guarantor spreading is its own article. Do not let a property model swallow the guarantor.

## Eight steps, two owners

The model does steps 2 through 7 only after step 1 is complete, and step 8 is a person.

1. **Assemble.** Rent roll, T12, leases with exhibits, sales reports if they exist, offering memorandum, appraisal, environmental report, and sponsor returns. Missing pieces are listed, not skipped.
2. **Ingest.** Classify documents. Flag what is absent. Do not let the tool organize a story the packet does not support.
3. **Normalize the rent roll and abstract the leases.** Expirations, co-tenancy, percentage rent, options, recoveries.
4. **Spread the T12.** Separate recurring and one-time items. Cite every adjustment. See the T12 article.
5. **Retail risk.** Occupancy cost where sales exist. Co-tenancy exposure under a scenario the analyst defined. Percentage rent only from reported sales.
6. **Sponsor.** A separate spread. Global cash flow, not a paragraph in the property memo.
7. **Stress.** Rate, rollover, vacancy, tenant-improvement and leasing-commission reserves, and reserve drag. Each case uses assumptions a person wrote. "DSCR, LTV, and Debt Yield" is the lender math those cases feed.
8. **Sign.** The reviewer checks citations, applies local knowledge the packet does not contain, and makes the call. The draft is not the call.

## Citations, or it did not happen

If a model invents an expiration, a cap rate, or a co-tenancy trigger, the error can sit inside a clean workbook until after closing. The control is dull. Every material extracted figure names a document and a page, cell, or section. A figure with no source is a flag, not a value. The reviewer can open that page. The investment memo can too. "The Audit Trail" is the same rule outside real estate.

Questions a later reader will ask, and the evidence that answers them:

| Question | Evidence in the file |
|---|---|
| How was NOI built? | T12 bridge, each line cited |
| How was debt service coverage stressed? | Baseline plus named scenarios |
| Were co-tenancy clauses found? | Abstract with trigger and the rent exposed |
| Was the sponsor read? | Separate spread, not a sentence |
| Where did a person change the draft? | Override log: name, time, reason |

## Metrics the model may compute, and may not choose

| Metric | Formula | A screen, not a covenant | The model's job |
|---|---|---|---|
| NOI | Effective gross income minus operating expenses | Deal-specific | Normalize and cite |
| Cap rate | NOI ÷ price | Often discussed around 6–9 percent for retail; the market is local | Compute from the NOI a person accepted |
| DSCR | NOI ÷ annual debt service | Lenders often start at 1.25× | Run scenarios from given assumptions |
| LTV | Loan ÷ value | Often 60–75 percent in retail conversations | Show the appraisal's rent basis against in-place rent |
| Occupancy cost | Occupancy cost ÷ sales | Screens above | Compute only where sales were provided |
| Rollover | Expiring rent ÷ gross potential | A clump in one year is the issue | Build the schedule from the leases |
| Co-tenancy exposure | Rent at risk if a named trigger hits | Disclose | Add only the clauses it actually read |

### The view from Arnould Blvd

On The Blvd Shopping Center, 101–149 Arnould Blvd, Lafayette, is roughly 63,000 square feet on two buildings, 27 units, with Command Platform as the lease record. This article does not underwrite it. No rent, NOI, or loan term is stated. The plate is the miss a model makes when the packet is only income and area. The center's recorded parking variance limits floor space to the parking the approval allows. A summary built from the rent roll alone will not see that. It will also not see that the corner bank parcel is not part of the center. The owner checks the recorded constraints. The model does not.

## The practical next step

1. Take the last acquisition or refinance packet and list every document the model was given. Write "missing" next to exhibits, sales reports, and the environmental report if they were not in the stack.
2. Pick one tenant and fill the percentage-rent table from the lease, or write "no sales report" and stop the occupancy-cost line.
3. Search the leases for co-tenancy. If the model abstract has none, confirm that by reading, not by trusting the silence.
4. Start an NOI bridge with cited lines. Use the T12 article's shape. Do not paste a seller's NOI into the memo unchanged.
5. Put the signed page, the override log, and the governance guide in the same folder as the draft.

---

*Cypress Command builds practical AI-enabled operating systems for owner-led businesses — including the owners and operators of commercial real estate. This article is educational. It is not legal, tax, or investment advice.*
