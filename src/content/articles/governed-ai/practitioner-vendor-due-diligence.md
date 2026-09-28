---
title: "AI Vendor Due Diligence Before an Underwriting Tool Is Signed"
series: "The Governed AI Series"
part: "Part II — Keep It Accountable"
eyebrow: "KEEP IT ACCOUNTABLE"
deck: "A scored review for a vendor whose model will sit inside underwriting: transparency, bias evidence, security, the contract, and the red flags that stop the conversation."
author: "Cypress Command"
date: "2026-09-28"
read_time: "13 min"
desk: "run"
status: "review"
source: "practitioner-reference"
---

# AI Vendor Due Diligence Before an Underwriting Tool Is Signed

"Vendor AI Features: Questions to Ask Before Your Software Turns Them On" is the ten-question review for a toggle inside software you already pay for. This practitioner reference is the review you run before you sign a vendor whose model will influence underwriting: a score, a section maximum, evidence you insist on seeing, and a short list of answers that end the deal. Use the short article for the feature. Use this one for the procurement.

The score is an operating threshold for your file, not a regulatory pass mark. A vendor at the line is eligible for a contract conversation. The vendor is not thereby appropriate, and a high score does not move liability off your desk. If the model produces a discriminatory outcome and you relied on it, the exam and the borrower are still yours. Indemnity is a backstop counsel negotiates. It is not a program.

Complete the review before the vendor sees owner financials, and keep the completed scorecard. Five years is the planning default in this suite. Counsel may require longer. An internal model you built or configured is in scope too. You are the vendor. Score yourself.

## How the points work

Each criterion is yes (2), partial (1), or no (0). Partial is allowed only with a written fix and a date. Not applicable drops out of the denominator, and you write why. A no on a high-risk item is a red flag, not a bad quiz grade.

| Response | Points | Meaning |
|---|---|---|
| Yes | 2 | Evidence seen and accepted |
| Partial | 1 | A dated remediation plan, and not on a red-flag item |
| No | 0 | No evidence. Escalate if the item is marked high. |
| Not applicable | Excluded | Scope really does not include it |

Illustrative rule for this draft: advance to contract negotiation only at or above 70 percent of the applicable points, with zero unresolved red flags. Between 60 and 69 percent, or one or two red flags with a dated plan, you may continue only in writing, with counsel on the contract, and a reread inside 90 days. Below 60 percent, or three unresolved red flags, stop. The vendor can come back after the holes are closed; six months is a reasonable cooling-off so "we updated the PDF" is not the next meeting.

Section minimums below add up in the same spirit. They are floors for the conversation, not a grade you publish as certification.

## Transparency

If the vendor cannot explain the model, you cannot explain a file that used it. Bias testing and logs depend on this section.

| # | Ask | Risk | Evidence |
|---|---|---|---|
| 1.1 | Training sources disclosed | High | Data lineage |
| 1.2 | The data includes commercial property, not only generic credit | Medium | Dataset description |
| 1.3 | Architecture and algorithm type disclosed | High | Model card or technical note |
| 1.4 | Which features move the output | Medium | An explainability note a person can read |
| 1.5 | Outputs carry a range or a confidence indication | High | A sample output |
| 1.6 | Limits and known failures are written | High | A limitations statement |
| 1.7 | Versions and a change log exist | Medium | The log |
| 1.8 | No personal data in training without a lawful basis | High | A training-data statement counsel accepts |
| 1.9 | An outside review in the last 24 months | Medium | The report |
| 1.10 | A model card | Low | The card |

Section max 20. An illustrative section floor is 14. A no on 1.1, 1.3, 1.5, 1.6, or 1.8 is a red flag. A no on 1.8 stops the review until counsel has read it. A missing model card on 1.10 is only "low" if the same facts appear elsewhere. If they appear nowhere, treat it as 1.3 failed.

## Bias evidence

A vendor who cannot show a pre-deployment test and a monitoring cadence is asking you to rent their blind spot. The test you will run yourself is in "Bias Testing for AI-Assisted CRE Underwriting." This section asks whether they have done any of the work.

| # | Ask | Risk | Evidence |
|---|---|---|---|
| 2.1 | Pre-deployment testing across the relevant characteristics | High | The report |
| 2.2 | A disparate-impact analysis, with the screen they used | High | The analysis |
| 2.3 | Monitoring at least quarterly | High | The policy and a sample report |
| 2.4 | The method can be rerun | Medium | The method note |
| 2.5 | They will give you the results | High | The results, not a summary slide |
| 2.6 | A written fix path when a test fails | Medium | The procedure |
| 2.7 | An outside bias review is available | Medium | The report, or a contractual right to commission one |
| 2.8 | They tell you when they find a problem | Medium | The notice clause |
| 2.9 | The test covers the characteristics counsel listed for your product | High | A coverage matrix |

Section max 18. Illustrative floor 13. Red flags: 2.1, 2.2, 2.3, 2.5, 2.9.

## The frameworks they claim

A vendor aligned to NIST and silent on fair lending is not aligned for a credit use. Ask for evidence, and have counsel say which rows apply to you. Do not require a European conformity mark from a vendor who will never place a system on the Union market, and do not accept "NIST" as a substitute for ECOA if ECOA is the statute you actually live under.

| Framework | Why it comes up | What "evidence" means |
|---|---|---|
| EU AI Act | Creditworthiness uses can be high-risk; territorial scope varies | Counsel's view, plus whatever documentation the vendor has if they claim conformity |
| NIST AI RMF | A voluntary risk structure | A mapping to govern, map, measure, manage — specific, not a logo |
| ECOA | Credit discrimination and adverse action, when in scope | A fair-lending policy that mentions the model |
| Fair Housing Act | Housing-related decisions, when in scope | A statement you can test, not a sentence on the website |
| GLBA | Customer financial information, when in scope | Safeguards language and a security exhibit |
| ISO/IEC 42001 | An AI management system | A certificate or an honest gap note |

Score this block out of an illustrative 20 points, floor 14, with red flags on "no fair-lending story," "no security story," and "no human-oversight story." Three items, not a scavenger hunt: if the use can affect credit, if the file holds financial data, can a person override and stop the tool?

## Performance

A compliant model that is wrong is still a bad model. Ask for commercial-property evidence, not a generic accuracy badge.

| # | Ask | Risk | Evidence |
|---|---|---|---|
| 4.1 | Accuracy checked on CRE-like files | High | A validation report |
| 4.2 | Out-of-sample results, not only the training fit | High | The results |
| 4.3 | False positives and false negatives defined for the decision you will use | High | The definition and the rates |
| 4.4 | Compared with a manual baseline | Medium | The comparison |
| 4.5 | Drift and retrain triggers | Medium | The monitoring policy |
| 4.6 | Metrics refreshed at least yearly | Medium | Last year's report |
| 4.7 | A report on your book, not only theirs | Low | A sample |
| 4.8 | A confidence line that forces human review | High | The escalation rule |

Section max 16. Illustrative floor 11. Red flags: 4.1, 4.2, 4.3, 4.8.

## Security and privacy

Owner tax returns, rent rolls, and personal financials are the file. Their store is your store for as long as the data sits there. "Data In, Data Out: What an AI Tool Should and Should Not See" is the internal rule. This section is the vendor's half.

| # | Ask | Risk | Evidence |
|---|---|---|---|
| 5.1 | A current SOC 2 Type II, or an equivalent you will accept in writing | High | The report, inside twelve months |
| 5.2 | Encryption at rest | High | The architecture note. AES-256 is a common bar, not a statute. |
| 5.3 | Encryption in transit | High | TLS 1.2 or newer is a common bar |
| 5.4 | Your data is not training fodder | High | A data-use clause |
| 5.5 | Deletion when the contract ends | High | The deletion clause, with a method |
| 5.6 | Breach notice on a clock | High | The clause. Seventy-two hours is a common contractual ask; the legal clock may differ. |
| 5.7 | Role-based access | Medium | The access policy |
| 5.8 | A penetration test on a yearly cycle | Medium | The summary you are allowed to see |
| 5.9 | Subprocessors listed and bound | Medium | The list |

Section max 18. Illustrative floor 13. Red flags: 5.1 through 5.6.

## Logs

When someone asks why the model leaned a certain way on a file, the answer is a log: the inputs, the version, the output, the time.

| # | Ask | Risk | Evidence |
|---|---|---|---|
| 6.1 | A decision log per file, with version and time | High | A sample |
| 6.2 | Version control | High | The practice, not the intention |
| 6.3 | A change process | High | The policy |
| 6.4 | You can get the logs | High | A contractual right |
| 6.5 | A way to produce records an examiner can read | Medium | The procedure |
| 6.6 | Retention at least as long as your schedule | Medium | Their policy next to yours |
| 6.7 | Docs updated within a set window after a change | Medium | An illustrative window is 30 days |

Section max 14. Illustrative floor 10. Red flags: 6.1 through 6.4.

## The contract

Counsel reads this section. You make sure the draft contains the asks before counsel has to invent them.

| # | Ask | Risk | Evidence |
|---|---|---|---|
| 7.1 | Liability for model error and discriminatory outcomes is addressed, not waived | High | The draft |
| 7.2 | Fair-lending indemnity is negotiated, not assumed | High | The clause |
| 7.3 | Professional liability insurance at a limit you set | High | The certificate. An illustrative ask in larger procurements is $5 million. Scale it to the book. |
| 7.4 | Cyber insurance at a limit you set | High | The certificate. Same illustrative figure, same warning. |
| 7.5 | An uptime commitment | Medium | The service level. 99.9 percent is a common draft, not a need. |
| 7.6 | A response time for a critical error | Medium | The service level |
| 7.7 | You can leave and take your data | High | Exit and portability |
| 7.8 | You can terminate for a compliance failure | High | The termination right |

Section max 16. Illustrative floor 11. Red flags: 7.1, 7.2, 7.3, 7.4, 7.7, 7.8.

A liability cap equal to one month of fees, on a tool that will touch multi-million-dollar recommendations, is a signal about how the vendor prices its own risk. Ask for uncapped liability on discriminatory outcomes, fair-lending violations, and data breaches. If the answer is no, write that down and let counsel tell you whether any cap you do accept is one you can live with. Do not discover the cap after an incident.

## The company

You will depend on them after the demo.

| # | Ask | Risk | Evidence |
|---|---|---|---|
| 8.1 | At least three years operating | Medium | A history you can check |
| 8.2 | Financials you are willing to rely on | High | Statements. Audited if the spend justifies it. |
| 8.3 | Three references in commercial property, not a cousin industry | High | Names |
| 8.4 | You called references they did not script | High | Your notes |
| 8.5 | An onboarding plan | Medium | The plan |
| 8.6 | Training for the people who will sign files | Medium | The curriculum |
| 8.7 | A roadmap that mentions regulatory change | Medium | The roadmap |
| 8.8 | A way they tell you when the law or the model moves | High | The notice process |

Section max 16. Illustrative floor 11. Red flags: 8.2, 8.3, 8.8. The eight sections as scored here total 138 points when you use the illustrative 20 for the framework block. Drop not-applicable items from the denominator before you compute the percentage. Applicable points divided into points earned is the only math that matters.

| Section | Max | Illustrative floor | Red-flag items |
|---|---|---|---|
| Transparency | 20 | 14 | 1.1, 1.3, 1.5, 1.6, 1.8 |
| Bias | 18 | 13 | 2.1, 2.2, 2.3, 2.5, 2.9 |
| Frameworks | 20 | 14 | No fair-lending, security, or override story |
| Performance | 16 | 11 | 4.1, 4.2, 4.3, 4.8 |
| Security | 18 | 13 | 5.1–5.6 |
| Logs | 14 | 10 | 6.1–6.4 |
| Contract | 16 | 11 | 7.1, 7.2, 7.3, 7.4, 7.7, 7.8 |
| Company | 16 | 11 | 8.2, 8.3, 8.8 |
| Total | 138 | — | — |

| Tier | Illustrative rule | Next step |
|---|---|---|
| Advance | At or above 70 percent, no open red flags | Negotiate. Evidence in the file before signature. A review 90 days after go-live. |
| Conditional | 60–69 percent, or one or two flags with a dated plan | Counsel on the contract. Reread in 90 days. Do not go live on a promise. |
| Stop | Below 60 percent, or three flags, or an auto-stop such as 1.8 | Keep the scorecard. Hear them again only after the failed items have evidence. |

Seventy percent is the floor of this procedure, not a compliment. Use the score to remove vendors. Choose among the ones who pass by references, by whether they have actually seen a retail rent roll, and by the contract.

## Questions operators ask

**We built it ourselves.** Score it. The obligations do not get lighter because the vendor is you.

**They will not send the model card or the bias report.** The refusal is a no. On a red-flag item, stop.

**How often do we rescore?** At selection, at renewal, and when the model, the training data, or their control claims change. Annual is a sound default for anything in live use.

**It only "assists."** If the desk usually follows it, treat it as decision support you are relying on. Run the full review. The human-oversight protocol is what keeps assistance from becoming the decision.

**They passed, then failed in production.** Exercise the termination right you insisted on. If the failure is fair lending or a breach, counsel leads the notice question. Keep the scorecard and the logs.

## The practical next step

1. Score the vendor you are closest to signing, including the nos. Do not leave blanks.
2. Put every red-flag no in a single list at the front of the file.
3. Send counsel the contract section and the liability cap, not the whole marketing deck.
4. Call one reference the vendor did not list, if you can find one. Write what they said.
5. If you are already live without this scorecard, fill it now and halt reliance on any red-flag hole until it is closed or formally accepted.

---

*Cypress Command builds practical AI-enabled operating systems for owner-led businesses — including the owners and operators of commercial real estate. This article is educational. It is not legal, tax, or investment advice.*
