---
title: "Property Management Software and Digital Twins: An Operator's Benchmark"
series: "The Shopping Center Operator Series"
part: "Part X — AI & Operating Systems"
eyebrow: "AI & OPERATING SYSTEMS"
deck: "What shopping-center math a property system has to do, where digital-twin claims outrun the evidence, and the order an owner builds capability. A buying guide, not a product pitch."
author: "Cypress Command"
date: "2026-09-28"
read_time: "15 min"
desk: "run"
lanes: ["operating-systems"]
status: "review"
source: "batch-e"
---

# Property Management Software and Digital Twins: An Operator's Benchmark

Retail property software is uneven. The lease math that makes a shopping center different — percentage rent, common-area reconciliations, sales reports, co-tenancy — is concentrated in a few large platforms and a handful of specialists. Many tools sold to small landlords keep the general ledger and skip that math. Drawings sold as digital twins are often floor plans with a new name. This article is a benchmark an owner can use before buying or before asking a team to build. It is not a recommendation of a Cypress Command product, and it does not specify one.

Vendor rows below are a reading of public product descriptions, compiled for operators. They are not a live test. Prices and checkmarks change. Confirm them on the vendor's current page before you rely on a cell.

## The gap that matters

An owner of a multi-tenant center needs three data sets joined: each lease's recovery rules, the general-ledger expenses those rules point at, and who occupied which space for how long. Generic commercial accounting often stores those apart. The failure mode is a perfect calculation under the wrong rule. Industry commentary has long said a large share of CAM reconciliations contain material errors even when the software can do the math. Treat that as a reason to test a bill, not as a statistic Cypress Command measured.

Published estimates of the property-management software market disagree by a wide margin, because each firm draws the category differently. A cautious reading is a market in the low billions of dollars, growing in the mid-single digits to high single digits. Do not use any one firm's total as your market.

## What to ask of the financial engine

**CAM.** A usable engine categorizes expenses at the account level, with includable and excludable flags by lease. It grosses up variable expenses to a stated occupancy, often 95 percent in retail forms, and does not gross up fixed expenses. It tracks caps, including the difference between a cumulative cap and a non-cumulative cap, and it separates controllable from uncontrollable costs when the lease does. It freezes a base year when the lease says so. It stores the denominator, the cap, and the allocation as fields on that lease version, so a tenant audit can be repeated. "CAM, NNN, and the Annual Reconciliation" is the operator version of the same bill. Software that recomputes from today's rules and cannot show last year's rules will lose an audit.

**Percentage rent.** Natural breakpoint is base rent divided by the percentage rate. An artificial breakpoint is a number in the lease. Illustrative only: base rent $90,000 and a 6 percent rate produce a $1,500,000 natural breakpoint. Sales of $2,500,000 would owe percentage rent on $1,000,000. Sales of $700,000 would owe none. The engine has to know which breakpoint the lease uses, which sales the tenant reported, and which deductions the clause allows. It should not invent sales.

**Clauses.** Co-tenancy, kick-out, and exclusive-use rights are triggers, not rent tables. A dark anchor can reduce inline rent, and those reductions can trip other clauses. One cited industry discussion puts an anchor going dark near a 50 percent rent reset within about a year. That figure is not a law and not a result from any center in this series. What is operationally true: almost no system turns "anchor notice" into a list of affected leases, a dollar exposure, and the notice dates. That list still lives in a spreadsheet. If you buy software, ask whether it can produce the list. If you build a workflow, build the list before you build a map.

## A reading of the landscape

Tiers are a shorthand. Enterprise platforms are deep and sold with a services project. Entry products publish a price and stop short of that depth. Specialists cover a slice. Small-landlord tools often have no percentage-rent engine at all.

| Platform | How it is sold | Percentage rent | CAM gross-up | Sales capture | API, as described |
|---|---|---|---|---|---|
| Yardi Voyager | Enterprise | Native | Full | Portal | Yes |
| MRI PMX | Enterprise | Native | Full | Workflow described | Yes |
| RealPage Commercial | Mid-market | Native | Full | Portal | Treat as unverified |
| Yardi Breeze Commercial | Published entry price | Basic | Basic | Basic | Limited |
| STRATAFOLIO | Specialist | Native | Yes | No | No |
| CRESSblue | Specialist | Native | Yes | No | Yes |
| Re-Leased | Specialist | Native | Yes | No | QuickBooks-oriented |
| AppFolio | Small landlord | No | Shallow | No | Yes |
| DoorLoop | Small landlord | No | Pro tier only | No | Yes |
| Buildium | Small landlord | No | Shallow | No | Yes |

Yardi's published Breeze Commercial price has been $2 per unit per month with a $200 monthly minimum, including a basic CAM and percentage-rent feature set and without a separate onboarding fee. That is an entry price with a ceiling: stacking plans, deal math, and the recovery-group depth of Voyager are not what that tier is for. Voyager is quoted. A UK public-procurement filing has been cited at £0.02 per square foot per year for a Voyager core; confirm the filing before you repeat the number. MRI's retail materials describe prorated breakpoints, offsets, and recoveries across specialty, anchor, and traditional leases, and a large installed base of commercial leases. Those are vendor descriptions.

The practical consequence: an owner can buy cheap retail math that will not go deep, or deep retail math that arrives as a project, or a specialist that omits an API, sales capture, or a visual layer. There is not, in this reading, a single shelf product that is retail-grade, transparently priced, and map-first. That is a buying fact. It is not a brief for any one builder.

## Digital twins, without the label

Call a twin by what it does.

| Tier | What you actually have |
|---|---|
| 0 | A static drawing |
| 1 | The drawing plus lease or sensor data on top |
| 2 | Live feeds |
| 3 | A model that can run a what-if |
| 4 | A system that acts on its own |

Most products marketed as twins are tier 0 or 1. For a small open-air center, on the order of 60,000 square feet, the evidence that is public and independent points at a data layer, not a cinematic model. Lawrence Berkeley National Laboratory has reported a median whole-building energy saving around 9 percent from fault detection, on the order of $0.24 per square foot per year, with a payback often discussed near two years. A multi-store HVAC case (BrainBox AI at Dollar Tree) has been reported against a weather-normalized baseline; read it as one firm's result, not as your utility bill. Full live 3D models are discussed as paying back on larger buildings, often above about 100,000 square feet. Vendor energy claims in this area often run hotter than the verified band. Ask for the method.

A sensible order for a small center, evidence first:

1. Water-leak sensors, where insurance or a short payback is real.
2. Fault detection on the HVAC you already have.
3. Occupancy sensing only if it changes a schedule you already run.
4. A three-dimensional model only if leasing or marketing will use it every week.

## The map is an interface only if the data is already true

Mall landlords have started coloring sales and rent on a floor plan inside large platforms. Spatial tools often say, correctly, that they complement the system of record. A map that does not show the lease, the CAM status, percentage-rent sales, and the open work order is a poster. Build or buy the financial record first. Hang the plan on it second.

If a vendor's drawing method is patented, ask counsel before you copy the method. That is a legal question, not a design preference.

## AI in the system of record

Several large vendors shipped agents that can create work orders, post charges, or send messages. Headline results are mostly theirs. One collection story with outside reporting is Brookfield's collections work: a move from about 97.6 percent to about 99.6 percent collected, on the order of two weeks faster, across a large building set, as reported in the trade press. Do not budget your center to that delta.

A JLL discussion of CRE pilots has been summarized as roughly 90 percent of organizations trying AI and about 5 percent hitting all of their stated goals. The pattern that matches "The Smallest Useful AI System" and "Where Human Review Belongs" is narrow scope, a write-back into the books you already keep, back office rather than tenant-facing, and a person on every amount and every legal notice. The pattern that fails is a broad rollout, a read-only dashboard, and a custom build with no owner.

Two guardrails belong in the data, not in a slide. Do not pool other landlords' non-public rent or sales to set price. That pattern is what the public enforcement conversation around revenue-management software has been about; counsel translates it for your use. And if a tenant-facing channel uses a model, say so. A 2025 renter survey (Rently, n=800) reported that a large majority lose trust when AI use is undisclosed. The sample is renters, not shopping-center tenants. The operating habit still holds: identify the draft.

## An owner's sequence

Ignore any roadmap that starts with a rendering. Sequence the work by what the audit needs.

1. **Documents in, a person checking.** Lease abstraction with citations. Highest leverage, lowest drama.
2. **CAM and percentage rent.** The math has to be right before a map has anything honest to show. Test one reconciliation by hand.
3. **A site plan joined to the lease record.** Occupancy, expirations, and arrears on the plan. The plan is a query, not a brochure.
4. **Clause exposure.** From a trigger to the leases it hits, the rent at risk, and the dates. Still mostly a spreadsheet. Make the spreadsheet a register.
5. **Sensors.** Water first. HVAC faults second. Skip a twin tier you will not operate.
6. **Any agent that writes.** One workflow, a named owner, a human gate on money and on notices. Last, not first.

"From Spreadsheets to Systems" is the stage path. "Building an Operating System for Property Management" is the weekly version. This article is the buying test those paths use when the center is retail.

### The view from Arnould Blvd

On The Blvd is 101–149 Arnould Blvd, Lafayette, roughly 63,000 square feet, 27 units, two buildings. Command Platform is the lease record used there. This article does not describe a sensor bill, a CAM true-up, or a software price for that property, and it does not announce a product. The plate is the join. Twenty-seven suites on two buildings are already a map. The map is useful on the day it shows the same expirations, recoveries, and open items the lease record shows. A rendering that cannot answer "what is Suite 4's co-tenancy" is a picture. The record remains the system.

## The practical next step

1. Write the three data sets your next CAM bill needs: lease rules, ledger accounts, occupancy by date. Note which of them your current tool cannot store.
2. Pick one percentage-rent lease and compute the breakpoint by hand. If the software disagrees, the software is not done.
3. Ask any vendor, in one email: gross-up of variable expenses only, cap history by lease year, sales entry, and an export of last year's bill. Keep the answer.
4. List clause triggers in a register before you commission a site-plan drawing.
5. If you pilot a model, use the smallest-useful-system test: one workflow, one owner, one measure, one review. No tenant-facing send without a person.

---

*Cypress Command builds practical AI-enabled operating systems for owner-led businesses — including the owners and operators of commercial real estate. This article is educational. It is not legal, tax, or investment advice.*
