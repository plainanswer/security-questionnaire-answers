# Certifications and compliance

The section a small vendor dreads, and the one where the pattern in
[../guides/answering-honestly.md](../guides/answering-honestly.md) does the most work. You are
going to write "No" several times in a row. That is survivable. What is not survivable is a
"Yes" you cannot evidence, or a "we're working towards SOC 2" that means nothing has started.

There is a longer treatment of this section in
[../guides/no-soc-2-what-to-say.md](../guides/no-soc-2-what-to-say.md).

`[[ FILL IN: ... ]]` marks a deliberate blank.

---

### Do you have a SOC 2 report?

**No.** We do not hold a SOC 2 report. [[ FILL IN: the position — e.g. At our current size the
cost is not proportionate, and we have chosen to put that money into the product. We document
our actual controls instead, which is what this response describes. ]] [[ IF TRUE: We would
consider certification at <specific trigger>. ]]

> Two failure modes to avoid. **One:** "SOC 2 in progress" when nothing is in progress — do not
> write it unless you have engaged an auditor and can name them. Reviewers ask which stage you
> are at, and there is no good answer to that if the honest one is "none". **Two:** apologising.
> You are a small vendor without a certification, which describes most of the software the
> reviewer's company buys. State it and move to what you *do* have.

---

### Do you have ISO 27001 certification?

**No.** We do not hold ISO 27001 certification, and we do not operate a certified information
security management system. The controls we do operate are described in this document.

---

### Are you GDPR compliant?

**Info.** [[ FILL IN: describe what you actually do — data minimisation, stated retention
periods, deletion on request, export on request, a published privacy policy, a named privacy
contact, subprocessors listed and disclosed. ]] Questions about our contractual and legal
position under data protection law are handled by [[ FILL IN: contact ]].

> **Notice this answer does not say "yes".** Whether a company is compliant with a body of law
> is a legal determination, not a checkbox a vendor gets to tick about itself — and a founder
> asserting it in writing is making a legal claim they are not in a position to make. Describe
> the practices; leave the conclusion to the lawyers. If a reviewer needs the assertion in a
> contract, that is a contract conversation.

---

### Which other frameworks do you comply with — HIPAA, PCI DSS, FedRAMP, CCPA?

**No.** We do not operate under [[ FILL IN: the named framework ]] and the product is not
designed for use cases requiring it. [[ FILL IN: if relevant — e.g. We do not store payment
card data ourselves; card processing is handled by <provider>. ]]

> If a buyer needs a framework you do not operate under, the deal may genuinely not be viable,
> and it is enormously better for both sides to establish that in week one. Saying so directly
> is a service to the reviewer, and they will remember it if their requirements change.

---

### Do you undergo any independent security assessment?

**No.** We have not undergone an independent security assessment or audit.
[[ FILL IN: what an assessor would find if they looked — the controls in this document,
dependency scanning, managed hosting, no in-house cryptography, and a small attack surface ]].

---

### Do you have documented information security policies?

**Info.** [[ FILL IN: honest version — e.g. We maintain written policies covering access
control, data handling and retention, secure development, backup and continuity, incident
response, and vendors, scoped to a company of our size. They are available on request. / We do
not currently maintain formal written policies. ]]

> If you say they exist, be ready to send them within a day, because the follow-up is "please
> attach them." A short set of true policies written for your actual company is far better
> received than a long generic set describing a security department you do not have — and a
> reviewer can tell which is which within about thirty seconds.

---

### When were your policies last reviewed?

**Info.** [[ FILL IN: date. If they were written recently, say so — "written <month year>" is a
perfectly good answer. ]]

> Undated policies read as unmaintained. Put a date on every document you send, and put a real
> one.

---

### Are you certified to any standard we have not asked about?

**Info.** [[ FILL IN: anything real — a national scheme, an industry attestation, a
certification held by your hosting provider that you are careful to attribute to *them* ]].

> If the honest answer is "none", write "none". This is the last chance in the section to claim
> your host's certifications as your own, and it remains the wrong move — see
> [03-hosting-and-infrastructure.md](03-hosting-and-infrastructure.md).
