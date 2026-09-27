---
title: "Data In, Data Out: What an AI Tool Should and Should Not See"
series: "The Governed AI Series"
part: "Part II — Keep It Accountable"
eyebrow: "KEEP IT ACCOUNTABLE"
deck: "Decide what each AI use may read and where its output may travel, before the tool's default settings decide for you."
author: "Cypress Command"
date: "2026-09-27"
read_time: "7 min"
desk: "run"
---

# Data In, Data Out: What an AI Tool Should and Should Not See

Every AI use has two edges: the information that goes in and the output that comes out. Most tools set both edges by default, and the default is rarely a choice the owner made. This article gives you a data boundary worksheet: four classes of information, a rule for each, a scope for each register row, and an outbound check for everything a tool produces.

## Two edges of every use

The inbound edge is what the tool reads. That might be a file a person uploads, text pasted into a chat window, a folder the tool is connected to, or every record a software feature can reach.

The outbound edge is where the output goes and what it carries. A summary of a customer file contains that customer's facts. A draft reply built from three documents can repeat a detail from any of them. Output is input in a new shape, so controlling what goes out starts with controlling what goes in.

Neither edge is a technical question first. It is an operating question: for this step, what does the tool need to see, and who may see what it produces? The technology then has to match the answer. If it cannot, the use waits.

Nothing in this article certifies a tool or a vendor practice. The worksheet records the owner's choices. Where the information involved may carry legal or contractual obligations, the business should confirm those obligations with qualified advisors, and the worksheet should reflect what they say.

## Sort your information into four classes

Most owner-led businesses can sort their information into four classes. The examples below are for the regional title office used throughout this series, described here as illustrative.

| Class | Illustrative examples | May an AI use read it? | Condition |
|---|---|---|---|
| Public | Recorded documents, published fee schedules, the office's website | Yes | Output is still reviewed. Public does not mean fit to republish. |
| Internal | Procedures, templates, staff schedules, internal checklists | Yes, in tools on the register | The use has an owner and a reviewer |
| Confidential | Customer files, contract terms, pricing, employee records | Only in tools on the register, scoped to the file or task | The owner approves the use and the register row says so |
| Restricted | Account numbers, wire instructions, identification documents, passwords, anything the business has agreed to keep out of outside tools | No, by default | Any exception is approved by the owner in writing, after obligations are confirmed with qualified advisors |

Three rules make the classes work.

- **Scope by task.** A tool summarizing one file sees that file, not the whole drive. The narrowest input that does the job is the right input.
- **Class travels with the output.** A summary of a confidential file is confidential. A draft that quotes a restricted figure is restricted, wherever it lands.
- **Unknown means no.** If nobody can say what a tool keeps, where it sends inputs, or who at the vendor can see them, treat the tool as unscoped and keep confidential and restricted information out until the answers are in writing. "Vendor AI Features: Questions to Ask Before Your Software Turns Them On" covers those questions in detail.

## Scope by role, not only by tool

A business already decides who sees what. The bookkeeper sees payroll. The dispatcher sees the schedule. A vendor sees its own work orders. An AI tool should inherit the scope of the person using it, never widen it.

This is where connected tools need the most care. An assistant connected to a shared drive can often read everything the connection allows, which may be far more than the person asking the question is meant to see. Imagine a hypothetical eight-person accounting practice that connects an assistant to its full file server so staff can ask questions about procedures. A junior staff member asks about year-end deadlines, and the answer draws on a partner's compensation memo because the memo mentions the same dates. Nobody intended that. The connection allowed it.

The fix is to scope the connection to the folders the use needs, and to check whether the tool respects the permissions of the person asking. If it does not, the use stays at a narrower connection, or it waits.

For each register row, add a short data scope to the Reads column:

| Register row | Reads (class) | Scope | Output may go to |
|---|---|---|---|
| Search package extraction | Public and confidential | The open file only | Examiner, then the file |
| Payoff letter comparison | Confidential | The open file only | Closer |
| Status reply drafting | Internal only; no confidential or restricted text pasted in | The text the processor provides | Processor, then agent or lender after review |

## Data out: where output may travel

The outbound check asks one question per destination: what must be true before the output goes there?

| Destination | What must be true first |
|---|---|
| The person's own working file | Reviewed at the level set in the register |
| A colleague or another team | Class and scope still fit the recipient's role |
| A customer, vendor, lender, or tenant | A named reviewer has checked it, including that nothing from another file or customer appears in it |
| Public: website, marketing, articles, social posts | The owner has approved it, and nothing confidential appears, even where a document is technically public |
| Another AI tool | Treated as new input for that tool, with the same classification rules |

The customer row carries a specific hazard. A drafting tool that has seen several files can carry a name, a figure, or an address from one into a draft for another. Reviewers should check for that on purpose, and the review scope in the register should say so.

The public row carries another. Public record is a fact about where a document sits. Publishing is a decision. A recorded instrument can be pulled by anyone, yet the business may still choose not to repeat its terms in marketing or articles, because repetition changes who reads it and how.

### The view from Arnould Blvd

On The Blvd shows both edges. Inbound, Command Platform gives each role a different slice of the same records: the owner, the operator, vendors, and tenants each see a scoped view. A vendor sees its own work orders. A tenant sees its unit's maintenance items. Neither sees the rest of the file. An AI use built on those records should follow the same slices, so that what a party can learn through a tool is no more than what its role already allows. Outbound, this series follows a publishing rule of its own. The property's easements are recorded, and articles in this hub cite them by entry number and describe what they govern. Their dollar terms stay out of public writing, even though the documents are on record. If an AI tool were drafting an article from the property's records, that rule would belong in its register row, under "May not," in plain words.

## Keeping the boundary in place

A data boundary written once holds only as long as the habits around it. Three routines keep it in place.

- **Teach the classes by example.** Staff remember "no account numbers, wire instructions, or ID documents in the chat tool" far better than "no restricted information." Give each class two or three concrete examples from your own work, and post them where the drafting happens.
- **Recheck scope at the register review.** Connections widen over time. A tool granted one folder for a pilot is often granted the whole drive when the pilot ends. At each scheduled review, compare each row's written scope to the connection as it actually stands.
- **Treat a vendor change as a trigger.** When a vendor changes what its tool keeps, where it processes inputs, or which features read your records, the affected rows get reviewed before the next scheduled date, not after.

A hypothetical landscaping company shows why the first routine matters. Its crew leads photograph job sites and ask a chat tool to draft completion notes for customers. The photos sometimes show gate codes and alarm panels. Nobody meant to share them. A one-line rule with that example, taught once, closes the gap better than a paragraph of policy.

## The practical next step

1. Copy the four-class table and sort your ten most-used kinds of information into it, with at least one example for each class.
2. For every row in your AI use register, write the class of information it reads and the narrowest scope that does the job.
3. List every AI tool connected to a shared drive, inbox, or system, and check whether its connection is wider than the task needs.
4. Add the outbound check to the review scope of any use whose output reaches a customer, vendor, lender, or the public.
5. Write down one publishing rule, a class of information you will not repeat in public even when it is available, and share it with everyone who drafts outward-facing material.

---

*Cypress Command builds practical AI-enabled operating systems for owner-led businesses — including the owners and operators of commercial real estate. This article is educational. It is not legal, tax, or investment advice.*
