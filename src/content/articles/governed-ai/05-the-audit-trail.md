---
title: "The Audit Trail: Recording What AI Prepared and What a Person Changed"
series: "The Governed AI Series"
part: "Part II — Keep It Accountable"
eyebrow: "KEEP IT ACCOUNTABLE"
deck: "A short record of what AI prepared, what a person changed, and who approved it lets an owner reconstruct any AI-assisted decision later."
author: "Cypress Command"
date: "2026-09-27"
read_time: "7 min"
desk: "run"
---

# The Audit Trail: Recording What AI Prepared and What a Person Changed

Months after a decision, someone asks how it was made. A customer disputes a figure, a partner questions a recommendation, or the owner simply wants to know why a notice went out with a particular date. If AI prepared part of the work, the honest answer depends on a record: what the tool produced, what a person changed, and who signed off. This article gives you a seven-field audit record, a worked example, and a routine for reading the trail so it improves the work instead of just filling a folder.

## Why the trail matters more once AI is involved

Before AI, most business records captured the finished product. The signed letter went in the file. The approved quote went in the customer record. Nobody needed to know what the first draft looked like, because a person wrote it and the same person approved it.

AI-assisted work splits that moment in two. A tool prepares a draft, a summary, or a list of options. A person reviews it, changes some of it, and approves the result. If only the final version is kept, the business loses the most useful information it has about the tool: where its preparation was right, where it was wrong, and what a reviewer had to fix.

The trail serves three readers.

- **The owner**, who needs to reconstruct a decision and see who made it.
- **The process owner**, who needs to know whether a review point is set at the right level, as described in "Where Human Review Belongs in an AI-Enabled Workflow" from the Operating Systems Series.
- **The next reviewer**, who inherits the work and needs to know what the tool typically gets wrong.

None of this is a claim that a trail satisfies any outside requirement. Where regulation or contract terms may require specific records, the business should confirm its obligations with qualified advisors. The trail described here is an operating control: a way for the owner to see the work.

## The seven-field audit record

Each AI-assisted item gets one record. Keep it short enough that a busy reviewer will actually complete it. The table below lists the fields and what a good entry looks like.

| Field | What it records | A good entry |
|---|---|---|
| Item | The work product and its identifier | "Closing checklist, file 1142" |
| Register entry | Which AI use this belongs to | The line from your AI use register |
| Level | Prepare, recommend, or decide | "Prepare" |
| What AI produced | The draft or output, saved as produced | The original checklist, unchanged |
| What the person changed | The edits, in plain words or as a saved comparison | "Corrected payoff good-through date; added HOA requirement" |
| Who approved | A named person and the date | "J. Closer, 3/14" |
| Source used | The document or record the reviewer checked against | "Payoff letter dated 3/12" |

Two fields connect this article to earlier ones. The **register entry** field points back to "The AI Use Register: Writing Down Where AI Touches the Business," so every record ties to a use the business has already written down. The **level** field uses the three levels from "Prepare, Recommend, Decide: Three Levels of AI Involvement and Who Signs Each." A record at the prepare or recommend level should always name the person who made the call. A record that claims the AI decided something is a finding, because AI never holds the decide level.

### What not to record

A trail that captures everything becomes a trail nobody reads. Leave out routine internal drafts that never leave the team and carry no money, dates, or terms. Leave out the full conversation with the tool unless the conversation itself is the work product. Record the input, the output, the change, and the approval.

## A worked example at a regional title office

The following example is illustrative. A regional title office uses AI to prepare a closing checklist from incoming payoff letters and lender instructions. The register entry says the tool reads the file's documents, drafts the checklist, and does nothing else. The closer reviews every checklist with the source documents open.

On one file, the trail for a single closing looks like this.

1. The tool produces a checklist with eleven items. The original is saved as produced.
2. The closer compares it to the payoff letter and finds the good-through date copied from the wrong letter. She corrects it.
3. She adds a homeowners association requirement the tool did not extract, because it appeared in an email rather than a document.
4. She approves the checklist and records her name and the date.

Six weeks later, the seller's lender questions a payoff figure. The owner opens the record and sees the original checklist, the corrected date, the source letter, and the approver. The question is answered in minutes. More useful still, the process owner reads a month of records and notices that the good-through date is the field most often corrected. That tells the office where to focus: perhaps the intake step should label which payoff letter is current before the tool ever sees it.

The same pattern works outside real estate. Imagine a hypothetical dental group whose front desk uses AI to draft insurance pre-authorization summaries. The trail shows that reviewers keep correcting procedure codes on one type of claim. The fix is a better reference sheet for that claim type, not a new tool. Or consider an illustrative distributor that uses AI to draft replies to delivery complaints. The trail shows that reviewers rarely change the draft but often change the promised delivery date. That tells the owner the dates, not the tone, need a firmer source.

## Where the trail lives

The trail belongs where the work already lives. A separate spreadsheet that someone updates after the fact will fall behind within weeks. Look for these properties in whatever system holds it.

- **It keeps the original.** The AI output is saved as produced, before any edits. Overwriting the draft with the final version erases the most useful part of the record.
- **It survives.** A record that disappears when a browser closes, a session ends, or a subscription lapses is not a record. The trail must persist.
- **It can leave with you.** The business should be able to export its records in a readable format and keep them if it changes tools.
- **It names people.** "Approved" with no name attached is not approval. Every record carries a person and a date.
- **It links to the source.** The reviewer's source document is attached or referenced, so a later reader can repeat the check.

### The view from Arnould Blvd

When Command Platform was built for On The Blvd Shopping Center, persistence was a requirement from week one: a change made in the system had to survive a reload. The reasoning was plain. A tool that forgets teaches the team to keep the real records somewhere else. The platform also exports its records as portable snapshots, so the property's history is never locked inside a single vendor's product. Those two properties are the foundation any audit trail needs. If what was prepared and what was changed are both kept, and both can be exported, then a question asked months later about a clause summary or a first-pass notice from the AI concierge can be answered by reconstructing the record, not by relying on anyone's memory of it.

## Reading the trail

A trail that nobody reads is storage. Set a monthly routine for the process owner, about thirty minutes per AI use.

- **Count the changes.** For each register entry, how often did reviewers change the AI output, and which fields did they change most? A field corrected often is a candidate for a better source or a clearer instruction.
- **Watch for silence.** A reviewer who approves every item without changes for weeks may be reviewing well, or may have stopped looking. Pull a sample and check it yourself.
- **Look for level drift.** Items recorded at the prepare level that were approved without a named person, or items where the AI output went out unchanged and unreviewed, mean the level is slipping in practice. Restore the review before anything else.
- **Note new inputs.** A new form, a new lender template, or a new vendor can change the error pattern. The trail is where you will see it first.

Illustratively, an accounting firm that reads its trail this way might find that AI-drafted engagement summaries need almost no correction, while AI-prepared reconciliation notes are corrected on nearly every file. The owner now has a reason to lighten one review point and tighten the other, and a record that shows why.

## The practical next step

1. Pick one AI use from your register and add the seven-field record to it, starting with the next item it prepares.
2. Confirm that the original AI output is saved before a reviewer edits it. If your tool overwrites the draft, save a copy by hand until that changes.
3. Make sure every approval carries a person's name and a date, and that the reviewer's source is attached or referenced.
4. Check that you can export the records in a readable format today, not after you need them.
5. Put a thirty-minute monthly review on the process owner's calendar to count changes, check for silent approvals, and note any level drift.

---

*Cypress Command builds practical AI-enabled operating systems for owner-led businesses — including the owners and operators of commercial real estate. This article is educational. It is not legal, tax, or investment advice.*
