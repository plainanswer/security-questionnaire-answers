# The answer bank

Model answers for the questions that recur across enterprise security questionnaires, written
in the form that clears review at a small company: **a one-word position, the plain fact, and —
where the answer is No — the compensating control.**

Read [../guides/answering-honestly.md](../guides/answering-honestly.md) first. It is one page
and it explains the shape every answer here uses.

## How to use these files

1. **Find the nearest question.** Questionnaires ask the same things in different words; many
   entries list the variants they appear as. Match the buyer's *phrasing*, keep your *substance*
   identical every time.
2. **Fill in every `[[ FILL IN: ... ]]`.** These are deliberate blanks, not formatting errors.
   An answer that goes out with one still in it is worse than no answer.
3. **Read the `>` note under each answer.** That is where the reasoning lives — what the
   reviewer is actually asking, and the trap in the obvious answer.
4. **Delete what does not apply.** A shorter document that is entirely true beats a complete
   one that is partly aspirational.
5. **Keep the result in version control, dated.** Answering once and reusing is the entire
   point; answering from scratch each time is how substance drifts between two questionnaires
   from the same buyer.

## The sections

| File | Covers |
|---|---|
| [01-company-and-scope.md](01-company-and-scope.md) | Who you are, headcount, scope, subcontractors, key-person questions |
| [02-data-handling-and-privacy.md](02-data-handling-and-privacy.md) | Data categories, encryption, retention, deletion, export, AI training |
| [03-hosting-and-infrastructure.md](03-hosting-and-infrastructure.md) | Hosting, regions, environment separation, patching, monitoring |
| [04-access-control.md](04-access-control.md) | Who can reach production, MFA, secrets, offboarding, logging |
| [05-secure-development.md](05-secure-development.md) | Code review, dependency scanning, pen testing, disclosure, deploys |
| [06-backup-and-continuity.md](06-backup-and-continuity.md) | Backups, restore testing, RTO/RPO, continuity, key-person risk |
| [07-incident-response.md](07-incident-response.md) | Response plan, detection, on-call, breach notification, logging |
| [08-subprocessors-and-vendors.md](08-subprocessors-and-vendors.md) | The subprocessor list, vendor assessment, transfers, audit rights |
| [09-devices-and-endpoints.md](09-devices-and-endpoints.md) | Device encryption, MDM, BYOD, training, background checks |
| [10-certifications-and-compliance.md](10-certifications-and-compliance.md) | SOC 2, ISO 27001, GDPR, other frameworks, policies |
| [11-ai-and-automation.md](11-ai-and-automation.md) | AI features, model providers, data retention, automated decisions |

## Where these files deliberately stop

No DPA text. No contract clauses. No liability, indemnity, or notice-period language. Those are
questions about documents you have signed, and they belong with your lawyer — see
[../guides/questions-you-must-answer-yourself.md](../guides/questions-you-must-answer-yourself.md).

Working through these files does not make you compliant, certified, or audit-ready, and none of
it is legal advice.
