---
title: "One Payment Link per Unit, Without a Full Property System"
series: "The Operating Systems Series"
part: "Part II — Build What Helps"
eyebrow: "BUILD WHAT HELPS"
deck: "A building-wide pay link makes the memo line your rent roll. One link per unit makes the payment identify itself. A spreadsheet can hold that register until the work outgrows it."
author: "Cypress Command"
date: "2026-09-28"
read_time: "7 min"
desk: "run"
status: "review"
---

# One Payment Link per Unit, Without a Full Property System

Most small centers do not miss rent because they lack a property-management suite. They miss it because many tenants pay one link, and the only clue to who paid is a memo typed on a phone. Some memos are the trade name. Some are blank. The bookkeeper rebuilds the roll from bank descriptions, and the rebuild is wrong just often enough to make the delinquency list a guess.

You can fix that without a full property system. Give each unit its own payment link, or its own recurring invoice, and keep a register that ties the link to the lease. The payment arrives already identified. The spreadsheet is the system until it is not. This article is that setup: the columns, the monthly pass, what you still do by hand, and the signs you have outgrown it.

It is not a software recommendation and not a lease form. "Unit" means the suite on your rent roll. Do not invent a second numbering scheme for the link.

## The memo line is not a control

A single pay link is simple when there is one tenant. On a multi-tenant center it hides identity in free text. You cannot see which unit has not paid, and you cannot tell a partial from a tenant who paid someone else's amount.

That matching lands in the first days of the month, while ACH returns are still possible and grace periods are running. Someone compares bank lines to a roll and emails tenants to ask what they meant. The design let the tenant name the payment after the fact.

A link per unit reverses the order. You name the payment when you create the link. The tenant pays the link for that suite. The report comes back with your identifier on it. The memo can still be wrong. You are no longer reading it to decide which row to credit.

One job, checkable by a person: this dollar belongs to this unit for this month. Not lease administration, not CAM reconciliation, not a work-order portal. Those can wait. Identity cannot.

## The register

Keep one row per unit. A spreadsheet is enough. The columns below are the whole tool. Names in the example are placeholders, not tenants of any center.

| Unit label | Tenant legal name on the lease | Monthly total due | Link label | This month | Status |
|---|---|---|---|---|---|
| A-1 | Northline Dental, LLC | $2,400 | Link A-1 | 2026-10 | Received |
| A-2 | Sample Goods, LLC | $1,850 | Link A-2 | 2026-10 | Submitted |
| B-1 | Harbor Fitness, LLC | $3,100 | Link B-1 | 2026-10 | Partial, $1,000 |
| B-2 | (vacant) | — | Link retired | — | Vacant |

A few rules keep the sheet honest.

- **The legal name is the lease name.** Trade names change and get misspelled. The row uses the party that signed. If a related company pays, note it on the row. Do not rename the row to match the bank description.
- **Monthly total due is total rent.** Base plus recoveries billed this month, or the gross amount the lease says to draft. If you only put base rent on the link, you will collect the rest by apology. The field note "Total rent, not base rent" is the reason.
- **The link label is yours.** It can be the unit label. It should not be a processor's internal account number, and it should not be a bank's last digits. You do not need those on this sheet. Store processor details in the processor, not in a workbook that gets emailed.
- **Status is a closed list.** Expected, submitted, received, partial, returned, waived. "Received" means your rail rule says the money has cleared, not merely that a tenant pressed pay. See "ACH or Card: How Multi-Tenant Rent Actually Clears." Write the definition at the top of the sheet so the next person uses the same words.
- **Vacant units keep a row.** Retire the link so a stranger cannot pay a dead suite. A row with no link and a status of vacant is a cleaner record than a deleted row you cannot explain later.

Add a notes column if you need it. Do not add a second sheet for "special cases" that becomes the real register. Special cases are rows with a status.

## How the month actually runs

The register is a pass, not a dashboard. Four moments cover it.

**Before the draft.** A person confirms each occupied amount against the lease file or the rent roll you trust. A changed rent, a concession ending, an updated recovery estimate: each edit gets a reason in the notes. Then the link is set to that amount. A standing link is still one per unit. The amount due still lives on the row, or the tenant will pay last month's number forever.

**As payments arrive.** Credit the row the link names. A payment on Link B-1 is B-1 even if the memo says "rent." A check or a wire with no link is posted the same day, method in the note. The sheet is the book. The bank is the evidence.

**Partials and overpayments.** A partial stays partial. Record the amount and the open balance. An overpayment is not income and not a silent net against next month. Decide in writing whether it applies forward or goes back. Silent netting is how next month's delinquency list starts wrong.

**After the window.** When the ACH return window has passed, rows still expected, submitted, partial, or returned become the delinquency list. "The Weekly Operating Rhythm" already describes the touch on the day after grace. This register is what makes that touch about the right units.

AI can list rows whose amount changed, rows still submitted past your window, and a draft note for a partial. A person confirms the amount against the lease and changes the status. The model does not mark rent received, and it does not email the tenant.

## What you still do by hand

This setup will not calculate a late fee, reconcile the year's common-area costs, store the lease, hold a security deposit, or replace the rent roll as the control for term and area. It will show you who is past grace so a person can assess the fee the lease actually states. Leaving the other jobs out is the point. A register that also tries to be a lease file becomes a second lease file, and the two drift.

What you do by hand is the tie-out. Export the sheet when you close receipts. Match the received total to the deposit that hit the bank, less processor fees, less anything still inside a return window. One number, sheet versus bank, plus a list of timing differences. If you cannot tie it, you do not have a register.

Hand the export to whoever posts the books. They should not have to read memos. If they do, the link labels are not surviving the handoff. Fix that before you add columns.

## When the spreadsheet is no longer the system

Stop when the sheet is asked to do a second job, not when someone is embarrassed by a spreadsheet.

You have outgrown it when more than one property is sharing links by mistake, when percentage rent or a mid-month recovery means nobody trusts the monthly total, when two people edit the file and you cannot tell whose status won, or when exceptions outnumber ordinary receipts. Until then, a full property system mostly adds screens between you and the same four moments. Buy it when the second job is real.

The process owner is whoever confirms the amounts before the draft. If that chair is empty, the links go stale, and a stale link looks official. "The Missing Role in Most Automation Projects: The Process Owner" applies here even though the tool is a spreadsheet.

### The view from Arnould Blvd

A 27-unit center such as On The Blvd, roughly 63,000 SF at 101–149 Arnould Blvd, is large enough that one shared pay link would be a monthly reconstruction, and small enough that twenty-seven links fit on a page. The lease record in Command Platform is the place a changed rent should be read from. A payment link is not that record. It is a pointer back to it. Nothing in this article describes a live payment page, a processor account, or how any particular suite at that center pays. The constraint is the count: one identity per unit, chosen by the landlord, before the tenant types a note.

## The practical next step

1. List every occupied unit with the legal name on the lease and this month's total rent. One row each. Retire any shared "building" pay link once the per-unit links are live.
2. Create one link, or one recurring invoice, per row. Label it with your unit label. Do not put bank details or processor account numbers on the sheet.
3. Define the status words at the top of the sheet, including the day a submitted ACH becomes received.
4. Run one month: confirm amounts, credit only by link, list partials and returns as their own statuses, and tie the received total to the bank.
5. Write down the one condition that would make you leave the sheet. Do not shop for a property system before that condition is true.

---

*Cypress Command builds practical AI-enabled operating systems for owner-led businesses — including the owners and operators of commercial real estate. This article is educational. It is not legal, tax, or investment advice.*
