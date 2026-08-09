# AI and automation

A new section on questionnaires, and a fast-moving one. Buyers have started asking where their
data goes when a product has AI features, and whether a human is accountable for automated
decisions. Many vendors are answering these badly — not dishonestly, but by accident, because
the person filling in the form does not know what the model provider's data-retention terms
actually say.

Go and read your provider's terms before completing this section. Several changed their
defaults in the last two years, and the answer you remember may no longer be the true one.

`[[ FILL IN: ... ]]` marks a deliberate blank.

---

### Does your product use AI or machine-learning models?

**Info.** [[ FILL IN: Yes/No. If yes — which features, and whether models are third-party APIs
or run by you. ]]

> If the answer is no, say so plainly and skip the section. Do not describe a roadmap.

---

### Is customer data sent to third-party AI providers?

**Info.** [[ FILL IN: Yes/No. If yes — name the provider, say what is sent, and say whether it
is sent automatically or only when a customer uses a specific feature. ]]

> "Only when the customer clicks the summarise button" is materially different from "every
> document is sent on upload", and the reviewer needs to know which. Any provider named here
> belongs in your subprocessor list — see
> [08-subprocessors-and-vendors.md](08-subprocessors-and-vendors.md).

---

### Does the AI provider train on your customers' data?

**Info.** [[ FILL IN: check the provider's current terms and quote the position, e.g. "Data
submitted through <provider>'s API is not used to train their models under their published
terms, and is retained for <period> for abuse monitoring." ]]

> Quote the provider's terms rather than paraphrasing from memory. The retention-for-abuse-
> monitoring clause is common and frequently missed — the data is not trained on, but it is
> retained, and a reviewer who knows that will notice if you only mention the first half.

---

### Can customers opt out of AI features?

**Info.** [[ FILL IN: Yes/No, and how. If AI processing is not optional, say so clearly. ]]

> Enterprise buyers increasingly need this to be Yes. If it is No, better they hear it now.

---

### Are automated decisions made about individuals?

**Info.** [[ FILL IN: usually No for B2B tooling. If your product scores, ranks, filters or
otherwise makes decisions about people — candidates, users, customers — say so, and say whether
a human reviews the outcome. ]]

> This one carries legal weight in some jurisdictions. If your product makes decisions about
> people, that is a question for your lawyer as well as this form.

---

### Is any part of your business operated by AI agents?

**Info.** [[ FILL IN: answer yourself, plainly. If AI systems write your code, handle your
support, or run parts of your operation, say so and say what oversight applies. ]]

> **No template can answer this for you, and this one will not try.** The question is arriving
> on questionnaires now. It is asked in good faith and the only bad answer is an evasive one —
> a buyer who discovers it later, having asked and been told nothing, treats it as a
> disclosure failure rather than a technology choice.
>
> For what it is worth, the repository you are reading is maintained by an AI-operated
> business, and says so in its README. Being asked is not the problem. Being caught being
> vague about it is.

---

### Who is accountable for AI-related failures in your product?

**Info.** [[ FILL IN: name or role ]] is accountable for the product's behaviour, including
features that use models. [[ FILL IN: what oversight exists — e.g. outputs are shown to the
user for review rather than acted on automatically ]].

> "A human is accountable, and outputs are advisory rather than automatic" is the answer most
> reviewers are hoping for. If it is true for your product, say it in those terms.
