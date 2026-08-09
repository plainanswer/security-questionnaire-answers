# Hosting and infrastructure

Mostly factual questions with easy answers, and one genuine trap: a lot of founders claim their
hosting provider's certifications as their own. Do not. Say whose they are.

`[[ FILL IN: ... ]]` marks a deliberate blank.

---

### Where is the product hosted, and where is customer data stored?

*Also asked as: "Name your hosting provider and data centre regions."*

**Info.** Production runs on [[ FILL IN: provider ]]. Customer data is stored in
[[ FILL IN: country and region ]].

> Name the country, not just the provider. "AWS" is not a location and the reviewer will come
> back for the region.

---

### Do you manage your own servers, or is the platform managed for you?

**Info.** [[ FILL IN: e.g. We run managed services — the provider patches and maintains the
underlying platform; we are responsible for our application and its configuration. / We manage
our own virtual machines, including operating-system patching. ]]

> This determines who the reviewer holds responsible for OS patching, so it decides how they
> read your next several answers. Managed is a perfectly good answer and usually the safer one
> at this size.

---

### Is customer data transferred or accessed outside its stated region?

**Info.** [[ FILL IN: Yes/No. If any subprocessor — support tooling, error tracking, analytics,
email — operates outside that region, say so and name it. ]]

> The common accidental "no" here: production data sits in the EU, but the error tracker,
> support inbox, and analytics all sit in the US. That is a transfer, and it is exactly what
> this question is asking about. Cross-check against
> [08-subprocessors-and-vendors.md](08-subprocessors-and-vendors.md).

---

### Is your infrastructure certified — SOC 2, ISO 27001?

**No.** [[ FILL IN: company name ]] does not hold SOC 2 or ISO 27001 certification. Our hosting
provider, [[ FILL IN: provider ]], holds [[ FILL IN: their certifications ]], which covers the
physical and platform layer but not our application. What we do at the application layer is
described in this document.

> **The distinction in the second sentence is the whole answer.** Claiming your host's
> certifications as yours is the fastest way to lose a technical reviewer's trust, because they
> know the difference and it tells them you might not. Drawing the line yourself, before they
> do, has the opposite effect. See [../guides/no-soc-2-what-to-say.md](../guides/no-soc-2-what-to-say.md).

---

### Is production separated from development and test environments?

**Yes.** Production runs in [[ FILL IN: separate project/account/instance ]], separate from
development. [[ FILL IN: state whether real customer data is ever copied into development —
and if it is, say so ]].

> "We use a copy of the production database for debugging" is a real practice at this size. If
> you do it, say so and say what protects it, rather than answering the question you wish had
> been asked.

---

### Do you have network-level protections — firewall, DDoS, WAF?

**Partial.** [[ FILL IN: what actually exists — e.g. The service sits behind <provider>, which
provides DDoS protection and TLS termination. Only ports 443 and <N> are open; the database is
not reachable from the public internet. ]] We do not run a separate web application firewall.

> Most small products get DDoS protection and TLS from their CDN or platform without having
> chosen it deliberately. That still counts — describe what is in place, name what is not.

---

### Is your infrastructure defined as code, and are changes reviewed?

**Info.** [[ FILL IN: e.g. Infrastructure is defined in <tool> and versioned in our repository;
changes go through the same review process as application code. / Infrastructure is configured
manually through the provider console by <N> people. ]]

> The manual answer is not disqualifying at one or two people. Pretending otherwise is, because
> the follow-up is "please share your infrastructure repository."

---

### How do you monitor availability, and what is your uptime commitment?

**Info.** Availability is monitored by [[ FILL IN: tool ]], which alerts
[[ FILL IN: who, and by what channel ]]. [[ FILL IN: your uptime commitment, or that you do not
offer a contractual SLA ]].

> Not offering an SLA is a normal position for a small company — say it plainly here. Whether
> you *agree* to one for this customer is a commercial negotiation, not a questionnaire answer,
> and it should not be committed to in a spreadsheet.

---

### Are systems and dependencies kept up to date?

**Yes.** [[ FILL IN: e.g. Platform patching is handled by our managed hosting provider.
Application dependencies are updated on a <cadence> and on notification of a known
vulnerability, via <tool>. ]]

> Give the mechanism, not an intention. "We keep things up to date" is what everyone writes;
> "Dependabot opens PRs and we merge security ones within a week" is checkable.

---

### Do you maintain an asset inventory?

**Partial.** At our size the inventory is small enough to be explicit: [[ FILL IN: list the
actual systems — e.g. one production environment at <provider>, one database, one object
store, and the SaaS tools listed in our subprocessor list ]]. We do not run a separate asset
management system.

> This is a control designed for companies with a thousand laptops. The honest small-company
> version is a list, and a list is a legitimate answer to a question about an inventory.
