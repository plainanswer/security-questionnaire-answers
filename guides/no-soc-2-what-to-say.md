# You don't have SOC 2 and they've asked for it

The specific moment this repo exists for. A deal is progressing, someone forwards a
questionnaire or asks for "your SOC 2", and you have neither the report nor a plausible route
to one inside this quarter.

## First, the arithmetic, so the decision is a real one

SOC 2 as a solo or small founder is widely reported at **$10,000–30,000 per year** and
**roughly 200 hours** of your own time. A founder on Hacker News put the threshold plainly:

> "Stay here until you're losing deals with big-ish companies to the point where it's worth
> investing $10-20k and ~200 hours."

Source: <https://news.ycombinator.com/item?id=29099573>

So the question is not "should I get SOC 2 eventually". It is "can this deal be won without
it". Frequently the answer is yes, and the reason is that the certificate was never the point.

## What the buyer is actually trying to establish

The reviewer has to produce a defensible recommendation about whether using your product puts
their company at unacceptable risk. SOC 2 is a shortcut to that judgement — an auditor already
did the work, so they can point at the report instead of forming an opinion.

Absent the shortcut, they have to form the opinion themselves. That is more work for them, and
it is entirely possible. What makes it possible is a vendor who gives them specific, consistent,
verifiable answers. What makes it impossible is a vendor who is vague, inconsistent, or
evidently bluffing — because then the reviewer has nothing to write down except doubt.

An auditor, on the buyer's side of the table, publicly:

> "Even if your customer asks you to be compliant, you don't have to be if they care enough
> about your product. If you seem intent on getting things right, that's a big plus. Most of
> your competitors don't even know what SOC 2 is."

Source: <https://news.ycombinator.com/item?id=48146259>

That last sentence is the opportunity. The bar is not "certified". The bar is "visibly more
serious than the alternatives on the shortlist".

## What to say, in order

**1. Answer the question asked, without flinching.**

> No, we do not hold a SOC 2 report.

Not "we're SOC 2 aligned". Not "we follow SOC 2 principles". Reviewers read those as evasions,
because they are: neither phrase means anything an auditor would recognise.

**2. Give the reason, once, without apology.**

> At our size the cost — commonly $10–30k a year plus several hundred hours — is not
> proportionate to the company, and we have chosen to put that into the product instead.

This is a legitimate business decision and it reads as one. What does not read well is
embarrassment, and what reads worst is a vague implication that certification is imminent.

**3. Replace the shortcut with the thing it was a shortcut to.**

> What we can give you instead is a written description of the controls we actually operate,
> answers to your questionnaire that are specific enough to check, and a public security page
> that stays current. Everything in it is true today and I will tell you where the gaps are.

Then send it, and make sure the gaps are genuinely in there. A document with no "No" in it is
not credible from a company of three people, and its uniform positivity is itself a signal.

**4. Name the trigger, if there is one.**

> We would commission an audit at [a specific point — regulated data, a named customer count,
> a revenue threshold].

Only if true. An invented trigger is a commitment you will be asked about at renewal.

**5. Convert the blocker into a commercial conversation.**

> If a SOC 2 report is a firm requirement for this contract rather than a preference, tell me
> now and we can talk about what that would take.

Sometimes it is firm, and the deal is not available. That is worth learning in week one rather
than week nine. Often it is not firm — the requirement came from a template, and the reviewer
has discretion they will use for a vendor who has been straight with them.

## The three artifacts that do the work

None of these require a certificate, and together they answer most of a questionnaire before it
is sent:

1. **A public security page.** Subprocessors, data categories, processing region, security
   contact, and an explicit "what we do not have yet" section. That last section is not a
   confession — it is what makes the rest of the page believable, and it pre-empts a chunk of
   the questionnaire. See
   [what-goes-on-a-trust-page.md](what-goes-on-a-trust-page.md).
2. **A short written policy set**, scoped to your actual size. Access control, data handling
   and retention, secure development, backup and continuity, incident response, vendors. A
   two-page policy that is true beats a twenty-page one describing a company with a security
   department.
3. **An answer bank** — the recurring questions with your standing answers, in your words,
   version-controlled and dated. That is what the [answers](../answers) directory in this
   repository is for.

## What none of this is

Working through this does not make you compliant, certified, or audit-ready, and it does not
substitute for SOC 2 or ISO 27001. It is not legal advice. It gets a truthful, coherent,
internally consistent set of answers in front of a buyer inside a day instead of a fortnight —
which at this company size is usually the difference that decides the deal.
