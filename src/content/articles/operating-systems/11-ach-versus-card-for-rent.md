---
title: "ACH or Card: How Multi-Tenant Rent Actually Clears"
series: "The Operating Systems Series"
part: "Part II — Build What Helps"
eyebrow: "BUILD WHAT HELPS"
deck: "Card fees compound on a monthly draft. ACH costs less and can return days later. A landlord's rule says which rail is the default, which is the exception, and who pays the difference."
author: "Cypress Command"
date: "2026-09-28"
read_time: "8 min"
desk: "finance"
status: "review"
---

# ACH or Card: How Multi-Tenant Rent Actually Clears

A tenant who asks to "just put the rent on a card" is asking for a convenience. On a supply order, the fee is noise. On a multi-tenant center, the same fee is a slice of rent, every month, on every suite that uses it. ACH, a bank draft, is cheaper and slower to prove. It can look collected on Monday and come back on Thursday. This article is the operating choice between those two rails: an illustrative month of cost, why landlords default to ACH for contract rent, and a short rule for the card exception.

Nothing here is a payment-network rulebook or legal advice. Fee schedules change. Whether you may pass a card cost through is a lease question and a counsel question. The job below is narrower. Pick a default rail, price the exception, and do not book a draft as collected until it has had time to fail.

## The fee is a rent problem, not a checkout problem

Retail rent is a large, repeating amount. Total rent, not base rent alone, is the draft: base, plus the tenant's share of taxes, insurance, and common-area costs, as the field note "Total rent, not base rent" puts it. A percentage fee on that draft scales with the rent.

A card payment also feels finished. The tenant sees an approval. The office sees a deposit pending. Both can be wrong later. A card dispute can arrive weeks after you counted the cash. An ACH return usually announces itself sooner: the bank sent the money back, with a short reason. Different clocks, same need. The receipt is provisional until the window you set has passed.

A card can be a fair exception for a tenant who will not set up a draft, or for a small one-time bill. It is a poor default for contract rent. The default should be the rail whose cost fits on one line of the owner report, and whose failures already have a follow-up.

## What each rail is actually doing

**ACH** is a pull from a bank account the tenant has authorized. You submit a debit for a stated amount. The tenant's bank can send it back. Ordinary returns, such as insufficient funds, a closed account, or an account the bank cannot find, often show up within a few banking days. A claim that the debit was not authorized can arrive much later. The first is a collections fact. The second is a stop-and-review fact. The field note "The first five days after an ACH return" covers the near window. Do not treat "submitted" as "kept."

**A card** is an authorization on a card network. Approval is fast, which is why it feels safer. The cost is a percentage of the charge, often plus a small per-item amount, whether or not the tenant stays current next month. A later chargeback reverses the receipt and usually adds a fee. The dispute file, lease, invoice, authorization, goes to the person who owns payment disputes. It is not an office judgment to freelance.

Neither rail knows your rent roll. The processor knows an amount, a date, and an identifier you gave it. If that identifier is not the suite, you will spend the month matching memos. "One Payment Link per Unit, Without a Full Property System" is that matching problem. This article is the rail. Solve them separately.

## An illustrative month

The figures below are a teaching example, not a quote and not any live center. Assume a flat ACH fee of $0.75 per debit, and a card fee of 2.9% plus $0.30. Assume eighteen suites each drafting $2,400 of total rent. Your schedule will differ. Read it.

| Rail | Fee on one $2,400 draft | Fee on 18 drafts | About a year |
|---|---|---|---|
| ACH debit at $0.75 | $0.75 | $13.50 | $160 |
| Card at 2.9% + $0.30 | $69.90 | $1,258.20 | $15,100 |

The card column is about $15,100 a year on this illustration, before any chargeback fee. The ACH column is about $160. If the landlord absorbs the card fee, it is an expense. If the tenant pays it on top, it is a surcharge you need permission to charge. If nobody has decided, the processor decides, and the deposit is simply thinner.

Run the same table on your draft count and your schedule before you publish a "we take cards" line. Higher rents make the card column worse. Percentage fees do that. Returns and chargebacks are extra: a return fee, staff time to un-collect the rent, a dispute fee. Price the ordinary month, then keep a small reserve for the month that is not.

## Why landlords lean ACH for contract rent

The lean is practical, and it has limits.

- **The amount is large and known.** A percentage of a known monthly total is a standing cost. A per-item ACH fee stays dull, which is what you want a rent fee to be.
- **The relationship is a lease.** You already have a signed obligation to pay. You need a draft that matches the register, not a card dispute process acting as accounts receivable.
- **Failures are legible.** "Insufficient funds" is a sentence you can say to a tenant and a row on the delinquency list. You still follow the lease. You do not need a legal conclusion to know the cash is not there.
- **The books stay closer to the bank.** A cheap draft that sometimes returns is easier to reconcile than a charge that unwinds a month later, after you called the month closed.

ACH is not safer in every sense. You can debit the wrong account, the wrong amount, or a tenant who revoked authorization. Those are operator errors, which is why the per-unit register exists. ACH is also a poor tool for a prospect who has not signed, or for a charge you want paid before you hand over a key. A card or a wire can be the right tool there. The lean toward ACH is about recurring contract rent, not every dollar the center receives.

## Where a card still earns its fee

Keep a card path. Write down what it is for.

A card earns its place when the amount is small, the timing is once, or the alternative is not getting paid. An application fee, a minor bill-back, a prospect who will not wire: those are intelligible uses. A tenant already on ACH who wants monthly rent on a card is a different conversation. Either the lease allows a convenience fee and you charge it, plainly, on top of total rent, or you decline and point them back to the draft. Absorbing the fee and calling it tenant service is how the illustrative $15,100 disappears with no line on the owner report.

If a tenant pays part of a failed month by card, record a partial against that month's row. Do not convert the lease to a card account because one draft returned. A tenant whose bank cannot accept your kind of debit is an exception with an owner, in the sense of "Design for the Work That Does Not Go According to Plan": a suite, a reason, and a review date. It does not become the template for the next lease.

## A one-page rail rule

Write this on a single page and keep it with the rent register. It is an operating rule, not a lease form.

| Question | A workable answer |
|---|---|
| Default for monthly total rent | ACH debit, amount taken from the register, not from a memo |
| When a card is allowed | One-time amounts under a ceiling you set, or a named exception |
| Who pays the card fee | Stated in advance: tenant, as a separate line, only if counsel says the lease allows it; otherwise do not take the card |
| When a receipt becomes "collected" | ACH: after your stated return window with no return posted. Card: after approval, with chargebacks watched on a weekly list |
| Who may add an exception | One named person. A waiver is a row, not a favor |
| What AI may do | Draft the tenant note, flag a card draft above the ceiling, list suites still on the exception list. A person approves the rail |

AI belongs on the edge of this rule, not in the middle of it. A model can compare this month's drafts to last month's rails and point at the suite that quietly moved from ACH to card. It can draft the sentence that states the convenience fee. It cannot decide that the fee is permitted, and it cannot mark rent collected.

### The view from Arnould Blvd

On The Blvd is a roughly 63,000 SF, 27-unit center at 101–149 Arnould Blvd in Lafayette. At that count, rent is a set of drafts, not a single building payment. Command Platform keeps the lease record in one place, and the critical-dates board reads from that record. A payment rail still has to point back to the same row a person can open. Which processor clears those drafts, and which account they settle to, is an operating choice. It is not described here. The plate is the constraint: twenty-seven identities, one rent roll, and a fee rule you could explain without opening a dashboard.

## The practical next step

1. Pull your processor's fee schedule and price one ordinary month: ACH versus card, on your real draft count. Label the result illustrative until the schedule is in the file.
2. Write the one-page rail rule, including who pays a card fee and who may grant an exception.
3. List every suite currently paying monthly rent by card. For each, either move it to ACH or record it as a named exception with a review date.
4. Set the moment a draft becomes "collected" on your register, and do not close the month before that moment has passed.
5. Point the ACH-return follow-up at the field note "The first five days after an ACH return," and keep card disputes on a separate list with an owner.

---

*Cypress Command builds practical AI-enabled operating systems for owner-led businesses — including the owners and operators of commercial real estate. This article is educational. It is not legal, tax, or investment advice.*
