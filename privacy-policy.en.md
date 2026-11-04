# Privacy policy

[Français](privacy-policy.fr.md) · Version 0.2.7 · 2026-11-04

Lou is the personal AI assistant of one private individual, published here under the pseudonym **115** ("the owner").
This page says, plainly, what Lou reads, what it keeps, where, for how long, who else sees it, and how you can limit or erase it.
It describes Lou **as it works today**. Anything still being built is marked *(in progress)*. Every change is recorded in the [changelog](CHANGELOG.md).

## Who is responsible

The owner. Lou is a personal tool, not a company or a service offered to the public. It is not sold, carries no advertising, and does not
build profiles of anyone for anyone else. The owner answers every request about your data personally (see [Your choices](#your-choices)).

## What Lou reads

Only what reaches the owner, with the owner's permission:

- **The owner's conversations** on their messaging apps (for example WhatsApp, LinkedIn, Instagram, Messenger, iMessage), read through an app
  running on the owner's own computer. Read-only, except for messages the owner has approved one by one.
- **The owner's email**: for each email, the sender, recipients, date, subject, its text and its technical identifier.
  **Attachments are never opened.**
- **The owner's calendar**: event titles, times, places and the number of attendees.
- **Messages sent to Lou's own WhatsApp number.** Only the owner's messages are processed. If anyone else writes to that number, Lou records
  only that a message arrived and when, and never reads it.

## What Lou keeps

| What | Why | How it's kept |
|------|-----|---------------|
| Your name and how to reach you (phone number, email address, profile handle) as they appear in the owner's conversations | Recognise the same person across apps | Encrypted; looked up through a keyed fingerprint, never in clear |
| The messages you exchange with the owner (for email: subject and text, without attachments) | Remind the owner to answer, help prepare replies and meetings | Encrypted |
| A short note per conversation: where things stand, what each side still owes | So the owner doesn't have to re-read everything, and Lou can offer help | Encrypted; written from messages with sensitive details already removed; the owner can correct it; erased with the messages |
| Messages Lou drafted, whether the owner approved them, and whether they were sent | Accountability: every message has a record | Encrypted, with a tamper-evident fingerprint |
| An activity log: what happened and when (ids, times, statuses, costs) | Audits: anything Lou did can be traced | **Contains no message content.** Cannot be altered or deleted, even by Lou |

**Never kept:**
- notes or profiles containing sensitive information about you: health, political opinions, religion, sexual orientation, ethnic origin, and similar
  (Lou's notes on conversations are checked so they never contain any);
- **sensitive details in your messages**: an automatic check, run in the European Union, removes them before Lou's AI reads a message
  ("can't make it tomorrow, [personal reason]") and erases them from the copy that is stored. When the check can't run, the message is hidden from
  Lou rather than read. This includes **money details**, the owner's too: account balances, amounts, bank or card numbers, IBAN
  and salary are replaced by "[financial detail]", keeping only what is asked and by when;
- voice recordings, once transcribed;
- anything from people who chose the **no content** or **ignore** level (see below): their messages are dropped before they are stored.

## Where it is kept, and who else sees it

- **Storage:** on servers located in the **European Union**, and on the owner's own devices. Content is encrypted with keys held by the owner;
  the hosting provider cannot read it.
- **AI providers**, only for the excerpt needed for a given task, never your whole history:
  - **Anthropic** (Claude), a company based in the **United States**, prepares answers and drafts. Under its commercial terms, this data is not used
    to train its models.
  - **Mistral**, based in the **European Union**, for the privacy check that removes sensitive details from messages, and to understand what a message asks of the owner (their
    availability, a time agreed, a deadline) so Lou can give a heads-up; later, speech-to-text. It receives only messages a first set of rules
    flags, after sensitive details are removed.
- **Web searches:** for public, current information (a train's status, a company, a place), Lou can search the web through its AI provider.
  Searches are about public things: Lou is instructed never to put your name or details in one, and every search is recorded so the owner can check.
- **The platforms the messages already go through:** WhatsApp (Meta) for Lou's own number, and Google for the owner's email and calendar,
  accessed through their official interfaces with the owner's permission.

Nothing is sold or shared for advertising. Nothing is published.

## How long

- Messages, emails, drafts and the owner's chats with Lou: their **text is erased automatically after 12 months**, or earlier if you ask.
  What remains is a record without content (who wrote, when, whether a message was sent, and a fingerprint that proves what was sent
  without allowing anyone to read it again), kept with the activity log.
- Voice recordings: deleted once transcribed.
- The activity log: kept **3 years**, because it is what makes Lou auditable. It holds no message content.

## Messages Lou sends

Lou writes to someone only when the owner asked for that message and approved the exact text. Each message is signed **"Lou"** (the first one links
here), unless it is the owner's own words. You can ask how any message was written: see the [Lou card](lou-card.en.md).

## Your choices

Everyone starts at **full**. You can change your level at any time; it applies as soon as the owner receives your request, and it is checked by plain
code before any AI is involved:

| Level | Lou writes to you | Lou keeps your messages | An AI reads your messages |
|-------|:---:|:---:|:---:|
| **full** (default) | ✓ (approved by the owner) | ✓ encrypted | ✓ |
| **no contact** | ✗ | ✓ encrypted | ✓ |
| **no content** | ✗ | only that you wrote, and when | ✗ |
| **ignore** | ✗ | ✗ | ✗ |

The owner can also, on their own initiative, set any of these levels for someone, or tell Lou never to read emails from a given address domain
(for example a medical office). You can also ask the owner to **see** what Lou holds about you, **correct** it, or **erase** it. Lowering your level erases what it no longer allows *(in progress: for now, ask for erasure as well)*.

**How to ask:** write to **lou.kernel@gmail.com**, reply to any message signed Lou, or tell the owner directly. The owner handles each request personally: opt-outs immediately, other
requests within 30 days. Each request is registered with its deadline and followed until it is answered. An erasure is prepared by Lou
and runs only once the owner has approved it; it removes the text of your messages, your name and your contact details, and keeps only a
record that messages existed and when, with your contact details as unreadable fingerprints so that your choices keep applying.

If you live in the EU, you also have the rights given by the GDPR, including complaining to your data protection authority.

## Security

Content encrypted at rest; a separate component, holding no AI access, is the only one able to send anything, and only messages the owner approved
(checked by a cryptographic signature); every step is recorded in a log that cannot be changed. Details of the infrastructure are deliberately not
published.

## Changes

This policy changes when Lou changes. Each version is listed in the [changelog](CHANGELOG.md), with what changed and why.
