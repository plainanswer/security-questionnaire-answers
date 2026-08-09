# How to answer a security questionnaire honestly when the honest answer is "no"

This is the method the rest of this repo applies. It is one page. Read it once and the
answer files will make sense.

## The mistake almost everyone makes first

A small company gets its first enterprise security questionnaire, reaches question 14 —
"Do you perform annual third-party penetration testing?" — and does one of three things:

1. **Says "yes" and hopes.** This is the only genuinely dangerous option. You have now put a
   false statement in writing to a company that may attach it to a contract. It is also the
   easiest to catch: the follow-up is "please attach the report."
2. **Says "no" and stops.** Truthful, and it reads as a gap with nothing behind it. Three of
   these in a row and the reviewer's summary writes itself.
3. **Writes a paragraph of hedging** that avoids saying either. Reviewers read a lot of these.
   Evasion is more visible from their side of the table than from yours.

## What works instead

> "'We don't have X' stalls; 'we don't do X — here's the compensating control' usually doesn't."

Every answer in this repo has the same three-part shape:

**1. A one-word position.** Yes, No, Partial, or Info. Say it first, before the explanation.
The person reading has 140 rows to get through and is scanning for the position, not the prose.

**2. The plain fact.** What you actually do. Specific, checkable, no adjectives. "Two people
have production access" beats "access is tightly restricted."

**3. The compensating control, if the position is No or Partial.** Not an apology — the thing
you do *instead*, and why it addresses the same risk at your size.

Applied to the pen-test question:

> **No.** We have not commissioned a third-party penetration test. Our application is a single
> service with no customer-configurable execution surface, dependencies are scanned for known
> vulnerabilities on every build, and we will commission a test before [[ FILL IN: the
> threshold — e.g. handling regulated data, or passing N enterprise customers ]]. If a test is
> a firm requirement for this contract, tell us and we will price it into the deal.

That answer costs you nothing. It is true, it shows you understand what the control is *for*,
and the last sentence converts a blocker into a commercial conversation — which is what the
reviewer wanted, because their actual job is to decide whether the gap is acceptable, not to
collect certificates.

## Why the reviewer is not your enemy

The person reading your questionnaire is usually not trying to disqualify you. They are trying
to produce a defensible recommendation. A vendor who says "no, and here is what we do instead"
gives them something to write down. A vendor who bluffs gives them a reason to escalate.

An enterprise auditor, in public, on a thread about exactly this problem:

> "Even if your customer asks you to be compliant, you don't have to be if they care enough
> about your product. If you seem intent on getting things right, that's a big plus. Most of
> your competitors don't even know what SOC 2 is."

Source: <https://news.ycombinator.com/item?id=48146259>

## The four positions, and when to use each

| Position | Use when | Trap to avoid |
|---|---|---|
| **Yes** | The control exists today, for all of the scope the question covers, and you could show evidence within a day. | "Yes" for something that is true of one system and not another. If it is partial, say Partial. |
| **No** | The control does not exist. | Stopping there. A bare No with no compensating control is the answer that stalls deals. |
| **Partial** | It is true of some systems, some of the time, or is in progress with a real date. | Using Partial as a soft Yes. If a reviewer would read your Partial as a Yes, rewrite it. |
| **Info** | The question has no yes/no answer — it asks *what*, *where*, or *how many*. | Padding. Answer the question asked and stop. |

## Consistency matters more than any single answer

The failure that actually costs deals at this size is not a weak answer. It is **two different
answers to the same question**, three weeks apart, because you wrote both from scratch.

> "Answer them once, version-control them, and response time drops from two weeks to two days,
> which is usually what keeps the deal alive."

Keep your answers in one file, in your repo, with dates. When a fact changes — a new
subprocessor, a new region, MFA finally enforced everywhere — change it in one place. Match the
buyer's *phrasing* every time; never let the *substance* drift.

## Three things you must not delegate

Not to this repo, not to a template, not to a language model:

1. **Anything about a contract** — DPAs, liability, data ownership, breach-notification
   deadlines, indemnities. These are questions about documents you have signed. Read the
   documents, or ask the lawyer who wrote them. This repo does not contain contract text and
   deliberately never will.
2. **Anything you have not verified this month.** "Backups are tested quarterly" is a claim
   about the past. If you cannot name when it last happened, the honest answer is Partial.
3. **Anything about a system you have not personally looked at.** Check the console. It takes
   four minutes and it is the difference between a statement and a guess.

## What this does not do

Working through this repo does not make you compliant, certified, or audit-ready. It does not
substitute for SOC 2, ISO 27001, or any other framework, and it is not legal advice. It gets a
truthful, internally consistent set of answers in front of a buyer in a day instead of a
fortnight — which, at this company size, is usually the difference that decides the deal.
