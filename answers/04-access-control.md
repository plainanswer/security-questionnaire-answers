# Access control

The section where a one-person company has genuinely strong answers and usually writes weak
ones. Many access controls exist to stop a large organisation losing track of who can do what.
If the answer is "one person, and it is me", the risk the control addresses is mostly absent —
say that, rather than trying to describe a process you do not have.

`[[ FILL IN: ... ]]` marks a deliberate blank.

---

### Who has access to production systems and customer data?

**Info.** [[ FILL IN: N ]] people have access to production systems: [[ FILL IN: roles ]]. No
one else, including [[ FILL IN: contractors, support staff, or whoever is genuinely excluded ]],
has access.

> Must match your answer in [01-company-and-scope.md](01-company-and-scope.md). Contradicting
> yourself between two sections of the same document is the most damaging error available here.

---

### Is multi-factor authentication enforced on administrative accounts?

**Yes.** MFA is enabled on [[ FILL IN: list the actual accounts — hosting provider, source
control, domain registrar, email, payment provider ]].

> Go and check each one now rather than answering from memory. This is the single most common
> place where a truthful-feeling "yes" turns out to be a "mostly". The **domain registrar** and
> the **email account** are the two people forget, and they are the two that let an attacker
> reset everything else. If any are missing, either fix it in the next ten minutes — it is
> genuinely that fast — or answer Partial and name the gap.

---

### Is access granted on a least-privilege basis?

**Info.** [[ FILL IN: e.g. Each person has the minimum access needed for their role.
Administrative access to production is held by <N> people. Application access for customers is
scoped to their own account's data. ]]

> If you are one person you hold all privileges by necessity. Say so: "The company is one
> person, who necessarily holds full access. There is no broader population to restrict." That
> is a complete and defensible answer, and it is better than describing a role matrix you do
> not have.

---

### How is access removed when someone leaves?

**Info.** [[ FILL IN: e.g. On departure we revoke access to <list of systems> and rotate any
shared credentials, on the same day. ]] [[ IF NOBODY HAS EVER LEFT — say so: "No one has left
the company to date; the process above is what we would follow." ]]

> Saying nobody has ever left is fine and reviewers accept it. Describing a well-oiled
> offboarding process that has never once run is a claim you cannot evidence.

---

### Do you review access rights periodically?

**Partial.** [[ FILL IN: e.g. With <N> people holding access, we confirm the list at <cadence>
rather than running a formal review cycle. ]] We do not operate a documented quarterly access
review.

> Partial, honestly explained, beats a Yes you cannot produce evidence for. The reviewer's
> follow-up to "Yes" is "please attach the last review."

---

### How are credentials and secrets stored?

**Info.** Shared credentials are stored in [[ FILL IN: password manager ]]. Application secrets
are held in [[ FILL IN: e.g. the hosting provider's environment/secret store ]] and are not
committed to source control.

> If you do not use a password manager, this is the cheapest gap in this entire document to
> close — most are free or a few dollars a month. Close it, then answer Yes truthfully.

---

### Do you enforce a password policy?

**Info.** [[ FILL IN: what the product actually enforces on customer accounts — minimum length,
whether you check against known-breached password lists, whether you offer SSO ]].

> Note that this question is often about *your customers'* passwords in your product, not your
> internal ones. Read which is being asked; some questionnaires ask both, several rows apart.

---

### Do you support SSO / SAML / SCIM for customer accounts?

**Info.** [[ FILL IN: Yes/No. If no, say whether it is on the roadmap and be honest about
whether it actually is. ]]

> This one is frequently a purchasing requirement rather than a security control. If the answer
> is no and the buyer needs it, better to find that out in week one than week six. Do not
> promise a delivery date in a questionnaire cell — that is a commercial commitment and it
> belongs in the contract conversation.

---

### Do you log administrative access to production?

**Info.** [[ FILL IN: what genuinely exists — e.g. Our hosting provider records an audit log of
console and API actions, retained for <period>. Application-level administrative actions are
recorded in <where>. ]]

> Be precise about the difference between *logging* and *alerting*. Most small setups record
> access but nobody is notified in real time. If nothing alerts you, do not imply that
> something does — the two words look interchangeable and are not.

---

### Can your staff access customer data in the product, and is that logged?

**Info.** [[ FILL IN: Yes/No — and if yes, under what circumstances, e.g. only to investigate a
support request from that customer, and whether the access is recorded ]].

> Almost every small SaaS has some form of support access to customer accounts. Reviewers know
> this. Describing it plainly, with whatever restraint you actually apply, reads far better
> than an implausible claim that nobody can ever see anything.
