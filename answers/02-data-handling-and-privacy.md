# Data handling and privacy

The section where vagueness costs you the most. The reviewer is building a mental model of
where their data goes and who can touch it. Every unclear answer here generates a follow-up
email, and follow-up emails are what turn a two-day review into a three-week one.

`[[ FILL IN: ... ]]` marks a deliberate blank. It must not go out as it stands.

---

### What categories of customer data do you store?

*Also asked as: "Provide a data inventory" / "What personal data is processed?"*

**Info.** We store: [[ FILL IN: the actual list — e.g. account details (name, email, company);
content the customer uploads or writes into the product; support conversations; billing records
(invoices and addresses, not card numbers); IP addresses and browser information ]].

> Write the real list, including the boring entries. Support email and server logs are personal
> data and everyone forgets them. A list that omits the obvious makes the reviewer wonder what
> else is missing.

---

### Do you collect more data than the product needs to function?

**No.** We store the categories listed above and no others. [[ FILL IN: if you collect anything
that is not strictly required — analytics, session recordings — name it here and say why ]].

> If you run session recording or product analytics, this is where it belongs. Reviewers find
> it in your privacy policy anyway.

---

### Do you store special-category or sensitive personal data?

**Partial.** This is not a category we intend to hold and we do not ask for it. We cannot fully
rule it out, because customers can type anything into free-text fields. We do not index,
analyse, or export those fields, and [[ FILL IN: what you do if it is reported to you ]].

> The honest answer for almost every SaaS product is Partial, not No. A flat "No" is a claim
> about what your customers type, which is not something you control. Reviewers who have seen a
> few of these recognise the honest version immediately.

---

### Is the product intended for, or knowingly used by, children?

**No.** The product is not intended for or knowingly marketed to children, and
[[ FILL IN: your minimum age term, if you have one ]].

> If you sell B2B software this is a two-second answer. Answer it and move on.

---

### Do you store payment card data?

**No.** We do not store payment card numbers on our own systems. Payments are processed by
[[ FILL IN: payment provider ]], which handles card data directly; we hold only the billing
records and the last four digits shown by that provider.

> The compensating control here is structural — you removed the risk rather than mitigating it,
> and it is worth saying so in those words. If you *do* store card numbers, stop reading this
> repo and go and talk to your payment provider.

---

### Is customer data encrypted at rest?

**Yes.** Customer data is encrypted at rest on [[ FILL IN: hosting provider and service ]].
[[ FILL IN: if backups are stored elsewhere, confirm those are encrypted too ]].

> Check this rather than assuming it. Most managed databases encrypt at rest by default and
> most self-managed volumes do not. Also check your *backups* — encrypted database, unencrypted
> backup bucket is the most common real gap behind a "Yes" on this line.

---

### Is data encrypted in transit?

**Yes.** All traffic to the product is served over HTTPS with TLS, and plain HTTP is redirected.
[[ FILL IN: if internal service-to-service traffic is also encrypted, say so; if it runs on a
private network instead, say that ]].

---

### How long do you retain customer data after an account closes?

**Info.** After an account closes we retain data for [[ FILL IN: period ]], after which it is
permanently deleted from production systems. Backups containing that data expire on their own
schedule and are overwritten within [[ FILL IN: backup retention period ]].

> The backup sentence is the part people leave out, and it is the part reviewers ask about.
> "Deleted immediately" is almost never true if you keep backups — say what actually happens.

---

### Can you delete all of a customer's data on request, and how quickly?

**Yes.** On request we delete a customer's data from production systems within
[[ FILL IN: your realistic turnaround, e.g. 30 days ]]. Copies in backups are not individually
removed; they age out as backups expire, within [[ FILL IN: backup retention period ]].

> Do not promise "immediately and everywhere" unless you have genuinely built selective
> deletion into your backups. Almost nobody at this size has. The above is the truthful version
> and it passes review routinely.

---

### Can a customer export their data in a usable format?

**Yes.** A customer can obtain their data in [[ FILL IN: format, e.g. JSON or CSV ]] via
[[ FILL IN: self-serve export / a request to support ]].

> "By emailing us and we run a script" is a legitimate answer at this size. Say which it is.

---

### Who owns the data a customer puts into the product?

**Info.** The customer does. We hold it in order to run the service for them.
[[ FILL IN: confirm this matches your actual contract terms before sending ]].

> **This is a contract question, not a security question.** Check the sentence against your own
> terms of service. This repo does not contain, draft, or interpret contract language, and you
> should be suspicious of any free resource that offers to.

---

### Do you use customer data to train AI or machine-learning models?

**Info.** [[ FILL IN: Yes/No — and if any part of the product sends customer data to a
third-party AI provider, name the provider and say whether that provider trains on it ]].

> This question is now on most questionnaires and it is frequently answered wrongly by accident
> — a founder answers "no" meaning "we do not train models", while the product sends customer
> text to a model API. Both facts belong in the answer. Check your provider's data-use terms
> before you write this one; several changed their defaults in the last two years. The provider
> also belongs in your subprocessor list — see
> [08-subprocessors-and-vendors.md](08-subprocessors-and-vendors.md).

---

### Do you have a privacy policy, and who is the data protection contact?

**Yes.** Our privacy policy is at [[ FILL IN: URL ]]. Privacy and data protection enquiries go
to [[ FILL IN: email address ]].

> Use a real monitored address. A privacy contact that bounces is worse than not listing one.

---

### Will you sign our Data Processing Agreement?

**Info.** [[ FILL IN: answer this yourself, with your lawyer. ]]

> **Do not answer this from a template — this one or anyone else's.** A DPA is a contract. This
> repo contains no contract text by design. Get the DPA from your lawyer, or use the standard
> one your own processors offer as a starting point for a conversation with one. What you can
> safely do here is say who to send it to and what your turnaround is.
