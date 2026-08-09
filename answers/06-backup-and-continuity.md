# Backup and business continuity

Two different worries wearing one hat. Backup questions ask "can you get the data back".
Continuity questions ask "what happens to us if you get hit by a bus" — and for a one-person
company that is a fair question with an uncomfortable answer. Answer it anyway; the founders
who address it directly do better than the ones who hope it goes unnoticed.

`[[ FILL IN: ... ]]` marks a deliberate blank.

---

### Do you back up customer data, and how often?

**Yes.** [[ FILL IN: e.g. The production database is backed up <daily/continuously> by
<provider>, retained for <period>. Uploaded files are stored in <service>, which is replicated
across <scope>. ]]

> Name the mechanism and the retention period. "Regularly" is not an answer; it is the absence
> of one.

---

### Are backups encrypted?

**Yes.** Backups are encrypted at rest by [[ FILL IN: provider/service ]].

> Verify rather than assume. Managed database snapshots are usually encrypted; a nightly dump
> you wrote yourself and pushed to object storage may not be. If it is not, fix it before
> answering — it is normally one configuration setting.

---

### Are backups stored separately from production?

**Info.** [[ FILL IN: honest version — e.g. Backups are held by the same provider in a separate
storage service and region. / Backups are copied to <second provider>. ]]

> Same provider, different region is the common real answer and is acceptable. Same provider,
> same region, same account is worth noticing yourself: it means one compromised account loses
> both. That is a gap worth closing before it becomes a questionnaire answer.

---

### Have you tested restoring from a backup, and when?

**Partial** *(unless you genuinely have)*. [[ FILL IN: honest version — e.g. We have restored
from backup as part of <specific event: a migration, a staging refresh, an incident> on
<date>. We do not run a scheduled restore test. ]]

> This is a question about the past, so it has a factual answer and you either have it or you
> do not. If you cannot name a date, do not claim a cadence. Better still: go and do a restore
> into a scratch environment this week, write down the date, and answer with it. It is a couple
> of hours and it converts three answers in this file from Partial to Yes — and, more to the
> point, it is the test that tells you whether your backups actually work.

---

### What is your recovery time objective (RTO) and recovery point objective (RPO)?

**Info.** [[ FILL IN: realistic numbers — e.g. Our target recovery point is <N> hours, matching
backup frequency. Our target recovery time is <N> hours for a full restore. These are targets
based on <the restore we performed / the provider's stated restore times>, not contractual
commitments. ]]

> Do not invent impressive numbers. A four-hour RTO you have never tested is a promise; a
> twelve-hour one derived from a restore you actually performed is evidence. The final clause
> matters — an RTO written into a questionnaire can end up referenced by a contract.

---

### Do you have a documented business continuity or disaster recovery plan?

**Partial.** [[ FILL IN: what exists — e.g. We maintain written recovery steps covering
restoring the database, redeploying the application, and communicating with customers. We do
not maintain a full business continuity plan of the kind larger organisations operate. ]]

> If you have nothing written, write the half-page version first, then answer. It is genuinely
> useful to you independently of any questionnaire: the worst possible time to work out your
> restore procedure is during the outage.

---

### What happens to our service if the company fails, or if key personnel become unavailable?

*Also asked as: "key person risk" / "vendor viability".*

**Info.** [[ FILL IN: the honest answer for your situation, which may include: a named person
with emergency access to critical accounts; documented recovery procedures; the customer's
ability to export their data at any time; how much notice you would give; whether source code
escrow is available on request ]].

> **This is the question a small vendor most wants to skip and most needs to answer.** The
> reviewer's real concern is being stranded, and the two things that genuinely address it are
> (a) the customer can export their own data at any time, and (b) somebody other than you can
> reach the accounts. If you have neither, that is worth fixing for your own sake, not the
> questionnaire's. Do not commit to escrow arrangements in a spreadsheet — say it can be
> discussed, and take it to the contract conversation.

---

### Do you have insurance — cyber liability or professional indemnity?

**Info.** [[ FILL IN: Yes/No and what type, or that you do not currently hold cyber liability
insurance. ]]

> A factual question about a policy you either hold or do not. If a buyer requires specific
> coverage, that is a commercial negotiation with a real cost attached — do not agree to it in
> a questionnaire cell.

---

### How would you notify us of extended downtime?

**Info.** We would contact [[ FILL IN: your named contact ]] directly by email, and post
updates at [[ FILL IN: status page or channel, or say you do not run one and contact customers
directly ]].

> Not having a status page is fine for a small customer base. Saying "we would email you within
> the hour" and meaning it is worth more than a status page nobody watches.
