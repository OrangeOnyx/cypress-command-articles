---
title: "Sponsor Financial Spreading with AI"
series: "The Governed AI Series"
part: "Part II — Keep It Accountable"
eyebrow: "KEEP IT ACCOUNTABLE"
deck: "A guarantor's cash flow is a document pile: the personal statement, the returns, the schedule of real estate, and the entities. The model extracts. A person decides which income is cash."
author: "Cypress Command"
date: "2026-09-28"
read_time: "16 min"
desk: "finance"
status: "review"
source: "batch-e"
---

# Sponsor Financial Spreading with AI

Sponsor spreading turns a borrower's papers into two outputs a credit file can use: global cash flow, and a net worth that separates liquid assets from everything else. The property's NOI does not answer whether the guarantor can carry a bad quarter. The papers do, if they are complete and if paper income is not mistaken for cash. A model is well suited to extraction across a stack of returns. It is poorly suited to deciding that a K-1 distribution happened. This article is that line. Amounts are synthetic. The sponsor is not a real person.

Governance of the file, including fair-lending and adverse-action questions when the use is credit to a person, sits in "AI Requirements for CRE Underwriting: A Complete Governance Guide." Do not treat the workflow below as a determination that any statute applies.

## Two outputs

Global cash flow adds the cash the sponsor can use and subtracts debt service across the portfolio, including the loan being asked for. Net worth lists assets and liabilities and then haircuts anything that is not cash. Lenders read both. A strong stated net worth with thin liquidity and large guaranties is not the same as cash.

Hand work on a complex sponsor is often a day or more: several hours on the personal statement, several on three years of returns, and more on entities and the schedule of real estate. An extraction pass can compress the transcription. It does not compress the judgment. Published "error rate reduced by 80 percent" claims are vendor math until your own override log shows them. Keep the log. Skip the slogan.

## Nothing starts until the stack is complete

The model will spread whatever it is given and sound finished. Missing documents are a stop.

| Document | Why it is here | What extraction may do | Ordinary gap |
|---|---|---|---|
| Personal financial statement | Stated net worth | List assets and liabilities; flag holes | Optimistic values, missing pages |
| Personal returns, three years | Income under penalty of perjury | AGI, Schedule C, Schedule E, K-1s | Amendments, missing schedules |
| Entity returns, three years | Whether the K-1 is real | Ordinary income, distributions, depreciation | Fiscal-year mismatch |
| Schedule of real estate owned | The rest of the portfolio | Map each asset to its debt | Omitted properties, old values |
| Organization chart | Who owns what | Percentages, circular ownership | Informal boxes |
| Operating agreements | Whether cash can come out | Distribution blocks, consents | Old agreements, side letters |
| Credit authorization | The report is not optional | None; a person orders it | Unsigned or expired |
| Contingent liabilities | Guaranties and disputes | Match to returns and entities | Silence |

Also stop on unreadable pages. A practical gate: if recognition confidence on a page is poor, a person reads it before any figure from that page enters the spread. Eighty-five percent is a teaching threshold, not a regulation. Pick a threshold and write it down.

## The personal statement is a claim

The statement is the sponsor's snapshot. The model's job is to argue with it.

| Asset | Check against | Liquidity | A flag |
|---|---|---|---|
| Cash | Recent statements | Liquid | A large balance with no statement |
| Brokerage | Statements | Liquid, with a haircut you choose | A number with no statement |
| Retirement | Statements | Not liquid | Counted as cash |
| Home | Assessment or appraisal | Not liquid | Stated value far above the assessment |
| Investment real estate | Schedule, appraisal, Schedule E | Not liquid | Missing from the schedule or the return |
| Business interests | Agreements, K-1 | Not liquid | A value many times the cash distributions |
| Notes owed to the sponsor | The note and the payments | Depends | No paper |

A teaching convention, not a rule of law: cap a self-reported real estate value at the lower of the stated number and 90 percent of the latest appraisal, unless a newer appraisal is in the file. The model can apply that cap. The person adopts the cap in the assumption log.

Liabilities fail by omission. Compare the statement with the credit report, the schedule's debt, and entity debt. A tradeline that is not on the statement is a question before the spread continues. Guaranties that are not listed are the same question. Borrowers more often leave a debt off than invent a bank account.

## Global cash flow uses cash

Depreciation is not cash leaving. Add it back when you are measuring cash to pay debt, and cite the line. A K-1 allocation is not cash received. Extract both the allocated income and the distribution. If they differ, the cash figure is the one that services debt, and the gap is a flag.

Illustrative sponsor, "Northline Sample Sponsor," not a real borrower:

| Cash item | Amount | Why this figure |
|---|---|---|
| Wages | $180,000 | Personal return |
| Schedule E cash, after adding back depreciation | $95,000 | Rental schedule; non-cash expense reversed |
| K-1 cash distributed | $40,000 | Distribution, not the $140,000 allocation |
| Cash income used | $315,000 | Sum of the three |
| Existing debt service | $210,000 | Schedule and credit report |
| Proposed debt service | $85,000 | The loan being asked for |
| Global cash flow after debt | $20,000 | 315,000 − 295,000 |
| Global DSCR | 1.07× | 315,000 ÷ 295,000 |

If the spread had used the $140,000 K-1 allocation instead of the $40,000 distribution, income would show $415,000 and coverage about 1.41×. The deal would look fine. The cash would not. Many institutional screens start around 1.20× global coverage. This teaching file fails that screen. The model should put 1.07× on the first page and name the K-1 gap as the reason, not bury it. The person, not the model, decides whether a 1.20× screen applies to this lender.

Stress the same page with assumptions you write: a 10 percent income cut, a 20 percent drop in stated asset values, a 200 basis point rate increase on floating debt. If a case pushes coverage under a floor you set (a teaching floor sometimes used is 1.10×) or net worth under the loan amount, the case goes to committee as a case, not as a surprise in the appendix.

Passive-loss carryforwards on Form 8582 can make today's income look durable when a future release changes it. Extract the carryforward and label it. Do not add it to cash.

## Returns check the story

Personal returns: adjusted gross income, wages, Schedule C, Schedule E rental, Schedule E pass-through, Schedule D, other income. Each with a page and line. Entity returns: the K-1 on the personal return should match the K-1 the entity issued. A mismatch is an explanation, not a blend. Three years side by side, with year-over-year jumps flagged, beat a single "average income" the model invented.

## Entities decide whether the guaranty is cash

Read the operating agreement for distribution waterfalls, preferred returns, consent rights, and transfer limits. A K-1 from an entity that cannot distribute is not liquidity. The model should list those clauses. Counsel reads what they mean. Cross-collateralization and a guaranty of affiliate debt belong on the contingent list, even when the sponsor's statement is silent.

## Eight steps

1. **Completeness.** Checklist signed. No extraction before that signature.
2. **Page quality.** Unreadable pages are read by a person or replaced.
3. **Personal statement.** Assets, liabilities, liquidity class, citations.
4. **Three years of returns.** Normalize depreciation and one-time items. Match K-1s to entities.
5. **Global cash flow.** Cash income, all debt service, coverage, the shortfall named.
6. **Entity map.** Ownership, blocks on cash, affiliate debt.
7. **Stress.** The cases above, rates written by the reviewer.
8. **Memo.** A senior person signs. The memo contains the cited spread, not a paste of raw output.

## Controls

| Control | What it prevents |
|---|---|
| Cited page and line on every figure | A number that was never in a document |
| No uncited figure in the memo | A hallucinated total that looks formatted |
| Human sign-off before committee | A draft treated as a decision |
| Credit report matched to the statement | A debt left off |
| Cash distribution used, allocation shown beside it | Paper income paying imaginary debt |
| Versioned file | A quiet edit after the meeting |

If the use is an adverse credit decision about a person, the reason has to be explainable. "The model declined it" is not a reason. That standard is in the governance guide. Build the citation habit before the first decline, not after an examination.

### The view from Arnould Blvd

On The Blvd, 101–149 Arnould Blvd, Lafayette, roughly 63,000 square feet, 27 units, two buildings, is a property, not a sponsor. Command Platform holds its lease record. This article states no guarantor, no tax return, and no net worth for anyone connected with it. The plate is the separation. Property NOI and sponsor cash are different spreads. A model that drops a sentence of "sponsor strength" under a retail NOI has not spread the sponsor. The person who wants the loan file opens the returns or does not claim the support.

## The practical next step

1. Write the document checklist and refuse extraction until it is signed.
2. On the last sponsor file, find one K-1 and write both the allocation and the cash distribution. If you only have one of them, the global cash flow is not done.
3. Match the personal statement's liabilities to the credit report. List omissions by name of the debt, not by a score.
4. Compute global coverage twice: once with cash distributions, once with allocations. Put both on the page. Use the cash one in the conclusion unless a person writes why not.
5. File the signed spread under the same governance folder as the property underwriting.

---

*Cypress Command builds practical AI-enabled operating systems for owner-led businesses — including the owners and operators of commercial real estate. This article is educational. It is not legal, tax, or investment advice.*
