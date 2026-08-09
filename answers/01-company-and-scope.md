# Company and scope

The opening section of almost every questionnaire. It looks like paperwork and it is not — the
reviewer is calibrating how much of the rest of the document to take literally. A one-person
company that says so plainly gets read more generously than one that writes in the first person
plural about its "teams".

Read [answering-honestly.md](../guides/answering-honestly.md) first if you have not.
`[[ FILL IN: ... ]]` marks a deliberate blank. It must not go out as it stands.

---

### Who are you and what does the product do?

*Also asked as: "Describe your organisation and the service being procured." / "Provide a brief
company overview."*

**Info.** [[ FILL IN: legal entity name ]] operates [[ FILL IN: product name ]], a
[[ FILL IN: one clause — what it does and for whom ]]. It has been in production since
[[ FILL IN: year ]] and is used by [[ FILL IN: rough customer count or "customers in
<industries>" ]].

> Keep it to three sentences. This is not the pitch; the reviewer already knows what you sell
> or they would not be reviewing you.

---

### How many people work at the company, and how many can access customer data?

*Also asked as: "Number of employees" / "Size of security team" / "How many staff have
privileged access to production?"*

**Info.** [[ FILL IN: N ]] people work on the product. [[ FILL IN: N ]] can access production
systems or customer data.

> Two numbers, no framing. If both are 1, write 1. Founders routinely try to soften this and it
> always reads worse than the number would have. A reviewer who sees "1" adjusts their
> expectations for the whole document; a reviewer who sees vagueness adjusts their trust
> instead. There is a follow-up question further down about not having a security team — answer
> it there, not here.

---

### Do you have a dedicated security team or a named security officer?

**No.** We do not have a dedicated security team. [[ FILL IN: name or role ]] is the named
point of contact for security matters and is responsible for the controls described in this
document. Security work is part of the engineering work rather than a separate function.

> If you are the only person, you are the named contact. That is a complete answer at this
> size. Do not invent a committee.

---

### What is the scope of this assessment — which systems and data does it cover?

*Also asked as: "Define the boundary of the service."*

**Info.** This assessment covers [[ FILL IN: product name ]], its production environment at
[[ FILL IN: hosting provider ]], and the customer data it processes. It does not cover
[[ FILL IN: anything genuinely out of scope — e.g. our marketing site, internal tooling that
holds no customer data ]].

> Scoping down is legitimate and expected. Scoping down to exclude something the buyer's data
> actually touches is not, and it is the kind of thing that surfaces later.

---

### Where is the company legally registered?

**Info.** [[ FILL IN: legal entity name ]] is registered in [[ FILL IN: country ]], company
number [[ FILL IN: registration number ]].

> Jurisdiction drives a lot of the reviewer's downstream questions about data transfer. Give it
> straight.

---

### Do you use subcontractors or freelancers with access to customer data?

**Info.** [[ FILL IN: Yes/No ]]. [[ IF YES — FILL IN: how many, what they do, and what access
they hold ]]. They are bound by the same confidentiality and access rules as anyone else
working on the product.

> If a contractor has production access, say so here. It will otherwise contradict your answer
> to the "how many can access customer data" question above, and inconsistency between two
> answers in the same document is the single most damaging thing in a questionnaire.

---

### How long has the product been in production, and how stable is the company?

*Also asked as: "Provide evidence of financial viability" / "What is your funding position?"*

**Info.** The product has been in production since [[ FILL IN: year ]]. The company is
[[ FILL IN: e.g. funded by revenue from customers / bootstrapped and profitable / financed by
<investor> ]].

> This question is about whether you will still exist in two years. It is a fair question. If
> you are bootstrapped and profitable, that is a *stronger* answer than a funding round, and
> most founders under-sell it. If your finances are genuinely not something you disclose, say
> that plainly rather than writing around it — and see the business-continuity question in
> [06-backup-and-continuity.md](06-backup-and-continuity.md), which is what they are really
> worried about.

---

### Is any part of your business or product operated by AI systems, and do you disclose it?

**Info.** [[ FILL IN: answer this one yourself. If AI systems operate part of your business or
make decisions affecting customer data, say so plainly and say where. If not, say that. ]]

> This repo will not answer this one for you, and neither will any template. It is appearing on
> questionnaires now and it will appear on more of them. Buyers increasingly ask, and finding
> out later is much worse than being told up front. Either answer is fine. Silence is not.
> See [11-ai-and-automation.md](11-ai-and-automation.md) for the questions that follow.
