# The questions no template should answer for you

This repository gives you model answers for most of a security questionnaire. This page is the
list of places where it deliberately stops, and why. If you take nothing else from this repo,
take this: the questions below are the ones where a copied answer does actual damage.

## 1. Anything that is really a contract question

**Which ones:** the DPA, liability and indemnity, data ownership, breach-notification
deadlines, audit rights, SLAs and uptime commitments, notice periods for subprocessor changes,
source code escrow, insurance requirements.

**Why this repo will not answer them:** they are questions about documents you have signed, or
about obligations you would be creating by answering. A questionnaire cell is a written
statement to a counterparty, and "we will notify you within N hours of a breach" typed into a
spreadsheet can end up referenced by the contract that follows.

This repository contains no contract text and no clause language, by deliberate design. Any
free resource offering to supply your DPA is offering you a legal document written by someone
who has never seen your business, your jurisdiction, or your terms.

**What to do instead:** ask your lawyer. For the DPA specifically, the standard agreement your
own processors publish is a reasonable starting point for that conversation — not a document to
forward as your own.

## 2. Anything you have not verified this month

**Which ones:** MFA coverage, encryption at rest (particularly on backups), log retention
periods, who currently has production access, whether a restore has actually been tested.

**Why:** every one of these is a claim about a live system's current configuration, and every
one of them drifts. The gap between "we enabled MFA everywhere" and "MFA is enabled everywhere"
is usually one account added in a hurry eight months ago.

**What to do instead:** open the console and look. Each of these is a two-to-four minute check,
and this is the single highest-value hour in preparing for a security review — not because the
questionnaire demands it, but because the answers are frequently not what you assumed.

## 3. Anything about your own AI use

**Which ones:** whether AI systems run part of your business, whether customer data reaches a
model provider, whether that provider retains or trains on it, whether automated decisions
affect individuals.

**Why:** only you know, the terms change, and this is the fastest-moving area on questionnaires
right now. An answer that was true when a template was written may not be true today.

**What to do instead:** read your provider's current data-use terms, then answer. And answer
plainly — a buyer who asks and gets vagueness, then finds out later, treats it as a disclosure
failure rather than a technology choice. See
[../answers/11-ai-and-automation.md](../answers/11-ai-and-automation.md).

## 4. Anything where the honest answer is bad for the deal

**Which ones:** a framework you do not operate under and cannot reach; a control the buyer has
made non-negotiable; a certification with a hard deadline attached.

**Why:** the temptation to soften is strongest exactly where the consequences of softening are
worst. A "yes" that unravels during contracting does not just lose the deal — it loses it
later, more expensively, and with your credibility attached.

**What to do instead:** say it in week one, and say what it would take. Some deals are not
available. Finding that out early is a good outcome, and the reviewer will remember which
vendor was straight with them when their requirements change next year.

## 5. Anything about a system you have not personally looked at

**Which ones:** any answer beginning "I think", "we should have", or "the provider probably".

**Why:** a questionnaire converts a guess into a written statement to a customer. That is a
category change, and it happens silently.

**What to do instead:** check, or answer Partial and say what you do not know. "We have not
verified this and will confirm within two days" is a legitimate thing to write in a
questionnaire, and it is far better received than a confident answer that turns out to be
wrong.

---

Everything else in this repository is a starting point you adapt. These five are not.
