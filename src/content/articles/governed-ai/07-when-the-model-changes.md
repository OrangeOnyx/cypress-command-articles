---
title: "When the Model Changes Under You: Reviewing AI Workflows After Updates"
series: "The Governed AI Series"
part: "Part III — Govern It Over Time"
eyebrow: "GOVERN IT OVER TIME"
deck: "Your documents stay the same when an AI model changes. The reader does not. A reference set shows what moved before real work does."
author: "Cypress Command"
date: "2026-09-27"
read_time: "7 min"
desk: "run"
---

# When the Model Changes Under You: Reviewing AI Workflows After Updates

An AI workflow that behaved well in March can behave differently in June without anyone at your business changing a thing. The vendor updates the model. The software adds a new instruction behind the scenes. A setting moves. The documents your team relies on have not changed, but the tool reading them has. This article gives you a reference set: a short list of questions with known answers that you run after every model or tool change, and a routine for deciding whether the workflow keeps its current review level, tightens, or pauses.

## The document stays put; the reader moves

Most business records are stable. A lease says what it says. A service contract carries the same dates it carried when it was signed. A policy manual changes only when someone edits it. An operator can reasonably expect that the same question asked about the same document will get the same answer.

AI tools do not offer that promise. The model behind a feature can be replaced or retuned by the vendor. The instructions the vendor wraps around your question can change. The way a tool splits a long document into pieces before reading it can change. Any of these can shift an answer, a summary, or the fields an extraction picks up, and the shift may be small enough that nobody notices for weeks.

This is not a flaw unique to any vendor. It is how these tools are built and improved. The governance response is simple: when the reader changes, check the reading.

## Three kinds of change to watch for

Not every update deserves the same attention. Sort changes into three kinds.

- **Model change.** The vendor announces a new or updated model behind a feature, or you switch providers. This is the largest change, and it calls for a full run of the reference set.
- **Tool change.** The software around the model changes: a new feature, a different way of attaching documents, new default instructions. Run the reference set for the workflows that use the changed part.
- **Input change.** Your own side moves: a new contract template, a new intake form, a new vendor's invoice layout. The model is the same, but it is reading something new. Run the reference questions that involve that input.

The question in "Vendor AI Features: Questions to Ask Before Your Software Turns Them On" about how you will know when a feature changes pays off here. A vendor that announces model updates gives you a date to act on. A vendor that does not means you need a standing schedule instead, such as a quarterly run regardless of announcements.

## Build a reference set

A reference set is a short list of real questions your workflow handles, each paired with an answer a person has already confirmed against the source document. It is your fixed yardstick. When the tool changes, you ask the same questions again and compare.

Keep it small. Ten to twenty questions per workflow is enough for most owner-led businesses. Choose them on purpose.

- **The routine case.** Questions the tool handles every week. These show whether everyday work still holds.
- **The high-consequence case.** Questions involving money, dates, and terms, where an error would be expensive or hard to reverse.
- **The known-hard case.** Questions the tool has struggled with before, found by reading the audit trail described in "The Audit Trail: Recording What AI Prepared and What a Person Changed."
- **The long-horizon case.** Obligations that run for years, where an error would sit quietly until the date arrives.

Record each question in a simple table.

| # | Question | Source document | Confirmed answer | Confirmed by | Last run result |
|---|---|---|---|---|---|
| 1 | When does the payoff for this file expire? | Payoff letter, file 1142 | Good through the 14th | Closer, 3/12 | Match |
| 2 | Which requirements must be cleared before closing? | Title commitment, file 1142 | Six items, listed | Examiner, 3/10 | One item missing |
| 3 | What notice period does the underwriter agreement require? | Underwriter agreement | As stated in the agreement's notice section | Office manager, 1/8 | Match, different wording |

The example is illustrative, drawn from the regional title office used throughout this series. Notice the third row: the answer matched in substance but used different wording. Record that. A change in wording is often harmless, but it is also the first sign that the tool is reading differently.

## Run it, compare it, decide

After a change, a named person runs the reference set and marks each result against the confirmed answer. Then the process owner decides what happens next. The table below is a starting point.

| Result of the run | What it suggests | Decision |
|---|---|---|
| All match | The change did not move this workflow's answers | Keep the current review level. Record the run. |
| Wording changes only | The reader shifted, but substance held | Keep the review level. Watch the audit trail closely for a month. |
| One or two substantive misses on routine questions | The tool now handles some everyday work differently | Tighten review to every item until a second run matches. |
| Any miss on a high-consequence or long-horizon question | The error would be costly or hard to catch later | Pause AI preparation for that question type. People handle it until the issue is understood. |
| Output format changed and breaks a downstream step | A handoff will fail | Pause the handoff. Fix the format before resuming. |

The levels from "Prepare, Recommend, Decide: Three Levels of AI Involvement and Who Signs Each" do not change after an update. The tool still prepares or recommends. A named person still decides. What changes is how much checking the preparation needs, and the reference set is how you set that on evidence rather than habit.

Two illustrative examples from other businesses show the routine at a small scale. A hypothetical property insurance agency runs its reference set after its email platform updates the model behind thread summaries. Every routine question matches, but one summary drops a renewal date mentioned deep in a thread. That is a long-horizon miss, so the agency pauses AI summaries for renewal threads and restores them only after a second run passes. Imagine, too, a small medical billing office whose document tool changes how it reads scanned forms. Two extraction fields now come back blank. The office tightens review to every form, reports the issue to the vendor, and reruns the set when the vendor ships a fix.

### The view from Arnould Blvd

Some obligations at On The Blvd Shopping Center run for years. The reciprocal access and parking servitude with the bank at the corner, recorded as Entry 2004-00057697, carries 13 bank spaces and expires on December 30, 2034. The critical-dates board already carries that date. The recorded document will say the same thing in 2034 that it says today. The AI concierge that reads it may not be the same reader by then. The concierge answers against the property's own records, which is the right design, but any answer it gives about a long-running obligation like this one belongs in the reference set and should be checked against the recorded source after every model or tool change. The document does not change. The reader might. A long-horizon question is exactly where a quiet shift would go unnoticed until the date arrived, so it gets checked first.

## Make it a standing cadence

The reference set is only useful if it runs. Tie it to a calendar, not to memory.

- **Run it after every announced model or tool change.** The person who owns each product, named in the vendor-feature review, triggers the run.
- **Run it quarterly regardless.** Some changes arrive without notice. A standing run catches them.
- **Add questions as you learn.** When the audit trail shows a new kind of correction, add a question that tests it.
- **Retire questions carefully.** A question can leave the set when the workflow it tests is gone, not because it keeps passing.
- **Keep the results.** Each run's results, dated and signed, are part of the audit trail. They show when a workflow was checked and what was found.

A reference set takes an afternoon to build and an hour to run. That is a small cost against the alternative, which is discovering a changed answer when a customer, a lender, or a date finds it first.

## The practical next step

1. Pick one AI workflow and write ten reference questions with confirmed answers, including at least two long-horizon obligations.
2. Name the person who runs the set and the person who decides what the results mean.
3. Find out how each vendor announces model or feature changes, and record the answer in your AI use register.
4. Run the reference set once this month to establish a baseline, and put a quarterly run on the calendar.
5. Adopt the decision table so that a miss on a high-consequence question pauses AI preparation for that question type until a second run passes.

---

*Cypress Command builds practical AI-enabled operating systems for owner-led businesses — including the owners and operators of commercial real estate. This article is educational. It is not legal, tax, or investment advice.*
