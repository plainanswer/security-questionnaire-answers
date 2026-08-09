# Devices, endpoints and people

Questions designed for an organisation with an IT department, a fleet of laptops, and an
onboarding queue. For a company of one to three people the honest answers are short, and the
temptation is to inflate them. Resist it — this section is where inflated answers are easiest
for a reviewer to test, because the follow-up is simply "show me the MDM console."

`[[ FILL IN: ... ]]` marks a deliberate blank.

---

### Are company devices encrypted?

**Yes.** [[ FILL IN: e.g. Full-disk encryption is enabled on all devices used to access
production systems or customer data (<FileVault/BitLocker/LUKS>). ]]

> Go and check it is actually on, on every machine including the old laptop you still use for
> travel. It is on by default on modern hardware and it is a two-minute check.

---

### Do you use mobile device management (MDM)?

**No.** We do not operate an MDM system. [[ FILL IN: what compensates — e.g. All devices with
access to production are company-controlled, encrypted, screen-locked, and running current
operating systems with automatic updates enabled. There are <N> such devices. ]]

> MDM is a control for a fleet you cannot personally inspect. With two laptops that you can
> look at right now, the risk it manages is largely absent — and naming the number of devices
> is what makes that argument land.

---

### Is anti-malware or endpoint protection installed?

**Info.** [[ FILL IN: honest version — e.g. Devices run the operating system's built-in
protection (<Defender/XProtect>) with automatic updates enabled. We do not run a separate
commercial endpoint protection product. ]]

> Built-in protection is a real answer and reviewers accept it. Do not name a product you
> installed once and disabled.

---

### Are operating systems and software kept patched on endpoints?

**Yes.** Automatic updates are enabled on all devices used to access production systems.

> One of the few questions in this section with an easy honest Yes. Verify it is actually on.

---

### Do employees use personal devices for work (BYOD)?

**Info.** [[ FILL IN: truthfully. If the same laptop is both your personal and work machine —
which is normal at this size — say so, and say what protects it: encryption, screen lock,
password manager, separate browser profile, no shared use. ]]

> Reviewers expect BYOD at this company size. What they want to know is whether anyone thought
> about it. A truthful "yes, and here is what applies to it" is much stronger than a No that a
> single follow-up question would disprove.

---

### Do staff receive security awareness training?

**No** *(most likely)*. We do not run a formal security awareness training programme.
[[ FILL IN: what compensates — e.g. The <N> people with access are the engineers who built the
system; MFA is enforced on all administrative accounts; credentials are held in a password
manager; we do not process payments or approve invoices by email instruction. ]]

> The last clause matters more than any training would: the attack that actually hits small
> companies is a convincing email asking someone to move money or reset a credential. Saying
> you have a rule against acting on emailed instructions is a specific, credible control.

---

### Are background checks performed on staff?

**Info.** [[ FILL IN: truthfully — e.g. We have not performed background checks; the company
consists of its founders. / Background checks are performed on staff with production access. ]]

> "The company is its founders" is a complete answer. Do not describe an HR process that does
> not exist.

---

### Are confidentiality agreements in place with staff and contractors?

**Info.** [[ FILL IN: Yes/No, verified against what has actually been signed. ]]

> A contract question. Check what was signed rather than what you intended to have signed. This
> repo does not supply agreement text.

---

### Is there a clear desk / clear screen policy?

**Info.** [[ FILL IN: the honest small-company version — e.g. Devices lock automatically when
idle and are not left unattended in public spaces. We do not operate an office. ]]

> If there is no office, say there is no office. It answers several questions in this section
> at once, and it is a legitimate answer rather than an evasion.
