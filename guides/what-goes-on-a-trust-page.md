# What goes on a security page

A public page at `yourdomain.com/security` is the highest-leverage hour of work in this whole
subject. It is a URL you can send the moment a security review starts, it answers a meaningful
share of a questionnaire before anyone fills one in, and — unlike a questionnaire response — you
write it once for every buyer instead of once per buyer.

## The contents

Drawn from what buyers actually ask for. A founder describing the same list from the buying
side put it as:

> "subprocessors, data categories, processing region, DPA link, security contact, and a short
> 'what we do not have yet' section."

### 1. What the product is, and who runs it

Two sentences. Company, product, size. If you are three people, say three people — the rest of
the page is read in the light of this number, and a reviewer who has to guess will guess
uncharitably.

### 2. Where data is hosted and where it lives

Provider, country, region. If backups live somewhere else, say where.

### 3. What data you hold

The categories, in plain words. Account details, customer content, support conversations,
billing records, logs. Include the boring ones — the omissions are what get noticed.

### 4. Your subprocessor list

A table: who, what they do, what data they can see, where they are. Dated. This is the single
most-requested artifact in an enterprise security review and the one small vendors least often
have ready.

Publish it as a page rather than a PDF, so you can update it in one place and point every
customer at the same URL.

### 5. How to report a security problem

A monitored address — `security@yourdomain` — and what a reporter can expect: acknowledgement
within a stated window, and updates until it is resolved. Do not offer a bounty unless you
intend to pay one.

### 6. The controls you actually operate

Short, specific, checkable. Encryption in transit and at rest, MFA on administrative accounts,
backup frequency and retention, dependency scanning, who can reach production. Six true lines
beat two pages of adjectives.

### 7. What you do not have yet

The section people leave off, and the one that makes the page work.

> **What we do not have yet.** We do not hold SOC 2 or ISO 27001 certification. We have not
> commissioned a third-party penetration test. We do not run a 24/7 on-call rotation. We do
> not offer SSO. Where a control is missing, the compensating measures are described above.

Three reasons to include it. It pre-empts questions that were coming anyway. It makes every
positive claim on the page more credible, because the page is visibly not marketing. And it
means a reviewer discovers your gaps in your words, on your page, with your compensating
controls attached — rather than in a call, from you, under pressure.

### 8. A date

"Last updated: 12 March 2027." An undated security page reads as abandoned, and a page dated
three years ago is worse than no page.

## What does not go on it

- **Contract text.** No DPA, no clauses, no terms. Link to where a buyer can request the DPA
  and route it to whoever handles your contracts. Publishing contract language you have not had
  drafted is a way to create obligations you did not intend.
- **Compliance claims you cannot evidence.** "SOC 2 aligned", "enterprise-grade security",
  "bank-level encryption". These phrases have no agreed meaning and reviewers discount the page
  the moment they appear.
- **Your hosting provider's certifications, presented as yours.** Name them and attribute them:
  "our hosting provider holds X, which covers the platform layer, not our application."
- **A trust-badge image.** Nobody has ever been reassured by one.

## Keeping it true

The page is a liability the day it stops being accurate — a buyer who finds a subprocessor in
your page source that is not on your list has found something worse than an incomplete list.

Put it in version control next to your answer bank, review it when you add a vendor or change a
region, and update the date. That is the whole maintenance burden, and it is roughly ten
minutes a quarter.

---

Publishing this page does not make you compliant, certified, or audit-ready, and none of it is
legal advice. It makes you a vendor whose answers are ready before the question arrives.
