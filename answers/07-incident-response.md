# Incident response

The section with the highest ratio of grand-sounding claims to actual capability. A reviewer
who has read a hundred of these can tell the difference between a response plan and a paragraph
about one. The good news: the small-company version of this control is genuinely achievable in
an afternoon, and once written it answers most of the section truthfully.

**One caution before you start.** Breach-notification timelines are set by law and by your
contracts, not by your preferences. Anything you write here about *when* you would notify
someone should match what you have actually signed and what applies where you operate. Check it
with your lawyer. This repo does not contain contract text or legal advice.

`[[ FILL IN: ... ]]` marks a deliberate blank.

---

### Do you have a documented incident response plan?

**Partial.** [[ FILL IN: what exists — e.g. We maintain a written incident response procedure
covering detection, containment, assessment, customer notification and post-incident review,
scoped to a company of our size. ]] We do not operate a staffed incident response function or a
24/7 on-call rotation.

> If nothing is written, write it before answering. Half a page covering *who decides, who is
> called, what gets shut off, who is told, and what gets written down afterwards* is a real
> plan at this size. A plan that fits on one page and is true beats a twenty-page one that
> describes somebody else's company.

---

### Who is responsible for handling a security incident?

**Info.** [[ FILL IN: name or role ]] is responsible for incident handling and decision-making.
[[ FILL IN: any external help you would call — hosting provider support, a security consultant,
your lawyer ]].

> Naming yourself is a complete answer. Naming who you would *call* is the part that makes it
> credible, because it shows you have thought past the first hour.

---

### How would you detect a security incident?

**Info.** [[ FILL IN: what is actually in place — e.g. Error and exception monitoring via
<tool>, uptime monitoring via <tool>, provider security notifications, and customer reports to
<security@ address>. ]]

> Be honest that customer reports are one of your detection channels. They are, for nearly
> every company of this size, and reviewers know it. Listing them as a channel is candour;
> omitting them and implying comprehensive automated detection is the kind of claim that
> unravels in a follow-up call.

---

### Do you have 24/7 monitoring and on-call staff?

**No.** We do not operate a 24/7 on-call rotation. Automated alerts from
[[ FILL IN: monitoring tools ]] reach [[ FILL IN: who, by what channel ]] at any hour, and are
responded to as soon as they are seen. [[ FILL IN: your realistic response expectation, e.g.
within business hours, and typically faster ]].

> A company of one cannot staff a rotation and should not claim to. The distinction that makes
> this answer work: alerts *arrive* around the clock even though a human may not act on them
> immediately. State both halves.

---

### What is your process for notifying customers of a data breach?

**Info.** [[ FILL IN: e.g. On confirming a breach affecting customer data we would notify
affected customers directly at their registered contact address, with what we know, what is
affected, and what we are doing. We would follow up with a written summary once the
investigation concludes. ]] Notification timelines applicable to us under law and under our
customer contracts take precedence over any general practice described here.

> Do **not** copy a specific hour count out of a template — including this one, which
> deliberately does not give you one. The applicable deadline depends on your jurisdiction,
> your role in processing the data, and what your contracts say. That is a question for your
> lawyer, and it is one of the very few places where getting it wrong has direct legal
> consequences.

---

### Have you experienced a security breach in the last N years?

**Info.** [[ FILL IN: truthfully. If no: "We have not experienced a breach of customer data."
If yes: state what happened, when, what was affected, and what changed as a result. ]]

> If something did happen, disclosing it with the fix attached is survivable and quite often
> respected. Concealing a breach that the buyer later discovers is not, and it converts a
> security question into a trust question.

---

### Do you conduct post-incident reviews?

**Info.** [[ FILL IN: e.g. After any incident affecting customers we write up what happened,
the cause, and what changed to prevent recurrence. These are kept in <where>. ]]

> Small companies frequently do this informally and then fail to claim it. If you write things
> down after an outage, that is a post-incident review — say so.

---

### Do you log security-relevant events, and how long are logs retained?

**Info.** [[ FILL IN: e.g. Application and access logs are retained for <period> by <provider>.
Provider-level audit logs are retained for <period>. ]]

> Check the actual retention setting rather than assuming. Several hosting platforms default to
> a few days on the free tier, which is shorter than most founders expect and shorter than most
> reviewers will like. If it is short and cheap to extend, extend it before answering.

---

### Would you support us during an incident investigation on our side?

**Yes.** We would provide [[ FILL IN: what you can realistically provide — relevant logs,
timeline information, and a point of contact ]] to support a customer investigation relating to
their own data.

> Keep this scoped to *their* data. Committing to unbounded forensic support for any customer
> incident is an open-ended obligation, and a questionnaire is the wrong place to accept one.
