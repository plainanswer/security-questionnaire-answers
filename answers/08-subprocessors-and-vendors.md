# Subprocessors and vendors

The single most under-prepared section, and the one where preparation pays off fastest. Almost
every founder underestimates their own subprocessor list by half, because they count the
database and forget the six SaaS tools that see customer data every day.

Build the list once, publish it, and this section answers itself for every buyer thereafter.

`[[ FILL IN: ... ]]` marks a deliberate blank.

---

### Provide a list of your subprocessors

*Also asked as: "List all third parties with access to our data."*

**Info.** Our current subprocessor list is published at [[ FILL IN: URL of your security or
subprocessor page ]] and reproduced here:

| Subprocessor | What it does | What data it can see | Where |
|---|---|---|---|
| [[ hosting provider ]] | Application hosting and database | All customer data | [[ country ]] |
| [[ object storage ]] | File storage | Customer uploads | [[ country ]] |
| [[ email provider ]] | Transactional email | Names, email addresses | [[ country ]] |
| [[ payment provider ]] | Payments and billing | Billing details, no card data held by us | [[ country ]] |
| [[ support tool ]] | Support conversations | Whatever customers write to us | [[ country ]] |
| [[ error tracking ]] | Error monitoring | Diagnostic data, may include identifiers | [[ country ]] |
| [[ analytics ]] | Product analytics | Usage events | [[ country ]] |
| [[ AI provider, if any ]] | [[ what it powers ]] | [[ what is sent ]] | [[ country ]] |

> **Work through this checklist before you claim the list is complete.** The ones people
> genuinely forget: error tracking, product analytics, the support inbox, transactional email,
> session recording, the CRM, the AI API, and any backup service separate from the host. If a
> vendor's system can display a customer's name, it belongs on this list.
>
> An incomplete subprocessor list is worse than a long one. Long is normal. Incomplete gets
> discovered when the buyer's own tooling flags a domain in your page source that is not on
> your list.

---

### How do you notify customers of changes to your subprocessor list?

**Info.** [[ FILL IN: e.g. The list at <URL> is dated and updated when it changes. Customers can
subscribe to notifications at <mechanism>, or we notify affected customers by email with
<period> notice before a new subprocessor begins processing. ]]

> Notice periods are frequently a contract term. Say what you do operationally; leave the
> committed notice period to the contract and to your lawyer.

---

### Do you assess the security of your vendors before using them?

**Partial.** [[ FILL IN: honest version — e.g. We select vendors on the basis of their
published security documentation and certifications, their data-processing terms, and the
regions they operate in. We do not run a formal vendor risk assessment programme. ]]

> "We chose providers that publish a SOC 2 report and process in the EU" *is* a vendor
> assessment, just an informal one. Describe what you actually consider, and be clear it is not
> a formal programme.

---

### Do you have data processing agreements in place with your subprocessors?

**Info.** [[ FILL IN: Yes/No per vendor, verified. ]]

> Check rather than assume. Most major providers publish a standard DPA that applies
> automatically or on acceptance; some require you to sign it explicitly, and it is worth
> spending an hour confirming which is which. **This repo does not supply DPA text and will not
> — it is a contract.** What you can do here is state, factually, which agreements are in
> place.

---

### Do any subprocessors process data outside the stated region?

**Info.** [[ FILL IN: Yes/No, and which. ]]

> Cross-check against the table above. This is the same trap as in
> [03-hosting-and-infrastructure.md](03-hosting-and-infrastructure.md): EU production, US
> support desk. Both are true; both need to be visible; and the reviewer will spot the mismatch
> if the two answers disagree.

---

### Can we audit you, or your subprocessors?

**Info.** [[ FILL IN: what you can realistically offer — e.g. We will answer questions in
writing, provide the documentation described here, and take part in a call. We are not able to
host an on-site audit, and we cannot grant audit rights over our subprocessors, whose own audit
programmes are described in their published documentation. ]]

> Audit rights are a contract term with real cost attached. Describe what you can practically
> do; do not grant rights in a spreadsheet. If the buyer insists, that is a negotiation for the
> contract, with your lawyer present.

---

### Do you resell or share customer data with third parties?

**No.** We do not sell or share customer data. The subprocessors listed above process data only
to provide the service, on our instructions.

> A clean, strong No that costs nothing — provided it is true. If you run advertising pixels or
> data-sharing analytics on the *product* rather than the marketing site, check that first.
