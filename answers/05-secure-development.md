# Secure development

Written for large engineering organisations, so several of these questions do not have a
sensible one-person answer. The compensating-control pattern does most of the work in this
section: name the risk the control addresses, then say what covers that risk at your size.

`[[ FILL IN: ... ]]` marks a deliberate blank.

---

### Do you follow a documented software development lifecycle?

**Partial.** [[ FILL IN: describe what actually happens — e.g. Changes are made on a branch,
tested, and deployed through an automated pipeline. Deployments are automated and reversible. ]]
We do not maintain a formal SDLC document.

> Naming the actual steps is worth more than the document the question asks for. You are
> answering the question behind the question: is code released deliberately, or by hand at
> midnight?

---

### Is code reviewed before it reaches production?

*Answer honestly — this is the question most often fudged by solo founders.*

**No** *(if you are the only engineer)*. With one engineer there is no second reviewer
available. Instead: [[ FILL IN: what compensates — e.g. all changes go through an automated
test suite and linting on every commit; deployments are automated and can be rolled back in
under a minute; database migrations are reviewed separately before release ]].

**Yes** *(if there are two or more of you)*. All changes are reviewed by another engineer before
merging to the main branch. [[ FILL IN: whether this is enforced by branch protection or by
convention ]].

> A solo founder who writes "Yes, all code is peer reviewed" has told a reviewer something
> arithmetically impossible given the "1 employee" answer six rows earlier. That contradiction
> is noticed, and it makes everything else in the document suspect. The No answer above costs
> nothing.

---

### Do you scan dependencies for known vulnerabilities?

**Yes.** Dependencies are scanned by [[ FILL IN: tool — e.g. Dependabot, npm audit in CI ]] on
[[ FILL IN: every build / a weekly schedule ]]. Security updates are applied within
[[ FILL IN: realistic window ]].

> If you are not doing this, it is free and takes about ten minutes to switch on for most
> stacks. Do it before you answer, then answer Yes.

---

### Do you perform static analysis or automated security testing?

**Partial.** [[ FILL IN: what runs — e.g. linting and type checking on every commit, secret
scanning on the repository ]]. We do not run a dedicated static application security testing
tool.

> Free secret scanning is available on most hosted source control and catches the failure mode
> that actually hurts small companies — a credential committed by accident.

---

### Do you commission third-party penetration tests?

**No.** We have not commissioned a third-party penetration test.
[[ FILL IN: the compensating controls — e.g. the application has a small, single-service attack
surface with no customer-supplied code execution; dependencies are scanned continuously;
authentication is handled by <provider> rather than implemented in-house ]]. We would commission
a test [[ FILL IN: at what trigger — e.g. before handling regulated data, or at <N> enterprise
customers ]]. If a test is a firm requirement for this contract, tell us and we will discuss it
as part of the commercial conversation.

> This is the worked example from [../guides/answering-honestly.md](../guides/answering-honestly.md).
> A pen test is a real cost — quoted anywhere from a few thousand upward — and pretending
> otherwise helps nobody. The final sentence turns a hard No into something the reviewer can
> escalate as a commercial question, which is often what they were hoping for.

---

### Do you have a vulnerability disclosure process?

**Info.** Security issues can be reported to [[ FILL IN: security@yourdomain ]]. We acknowledge
reports within [[ FILL IN: realistic window, e.g. two business days ]] and will keep the
reporter informed until the issue is resolved.

> Setting up a monitored `security@` address is a ten-minute job that answers this question
> permanently, and it belongs on your public security page too. Do not promise a bug bounty
> unless you intend to pay one.

---

### How quickly do you patch a critical vulnerability?

**Info.** [[ FILL IN: realistic targets you would actually hit, e.g. critical issues affecting
customer data are patched within <N> days of becoming aware; others in the normal release
cycle. ]]

> Pick a number you have actually met. A 24-hour commitment from a company of one, who
> sometimes takes holidays, is a promise you will eventually break in writing.

---

### Are developers trained in secure development practices?

**Partial.** [[ FILL IN: honest version — e.g. We do not run a formal training programme. The
engineer working on the product has <N> years of professional experience and follows <specific
practices — parameterised queries, framework-managed authentication, no hand-rolled
cryptography>. ]]

> "We do not run formal training" plus two concrete practices is a better answer than "Yes, all
> staff receive annual security training" when all staff is one person who did not.

---

### Do you use a framework or library for authentication, or is it custom-built?

**Info.** [[ FILL IN: e.g. Authentication is handled by <provider/framework> rather than
implemented in-house. ]]

> If you did not write your own authentication, say so prominently. It removes an entire class
> of risk from the reviewer's model and it is one of the strongest answers a small company can
> give in this section.

---

### How are changes deployed, and can they be rolled back?

**Info.** [[ FILL IN: e.g. Changes deploy through an automated pipeline from the main branch.
Any release can be rolled back to the previous version in under <N> minutes. Database
migrations are applied separately and reviewed before release. ]]

> Rollback speed is a genuine control and it is one small teams often do better than large
> ones. Claim it.
