# Privacy policy

[Français](privacy-policy.fr.md) · Version 0.2.13 · 2026-11-13

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
- **The owner's phone calls**, from the call history on the owner's own computer: who, when, which way, whether it was answered and how
  long. **Never what was said.** Only calls with people Lou already knows from the owner's messages; a call never adds anyone.
- **The owner's contacts**, only when the owner exports them to Lou: names, numbers and addresses, to put a name on people Lou already
  knows. Lou adds nobody from them and has no standing access to the owner's address book.
- **Messages sent to Lou's own WhatsApp number.** Only the owner's messages are processed. If anyone else writes to that number, Lou records
  only that a message arrived and when, and never reads it.

## What Lou keeps

| What | Why | How it's kept |
|------|-----|---------------|
| Your name and how to reach you (phone number, email address, profile handle) as they appear in the owner's conversations | Recognise the same person across apps | Encrypted; looked up through a keyed fingerprint, never in clear; two records with the same full name are treated as one person, and the owner can separate them |
| The messages you exchange with the owner (for email: subject and text, without attachments) | Remind the owner to answer, help prepare replies and meetings | Encrypted |
| Your phone calls with the owner: when, which way, how long | So Lou knows something may have been settled on a call, and asks the owner instead of guessing | Never what was said; only if Lou already knows you; erased with your data on request |
| A case file per person or organisation: where things stand, and what is still open between you and the owner (something to do, something awaited, a date agreed), each point with the messages it comes from | So the owner doesn't have to re-read everything, and nothing is forgotten or invented | Encrypted; written only from messages the privacy check has passed; a point that no message proves is refused by code; the owner can correct it, and Lou asks the owner when it can't know (a call, a meeting); erased after 12 months, or with your data on request |
| A contact card about you: your name and nicknames, birthday, how you relate to the owner and how close you are, your work, how you met, a one-line description, and the latest context | So Lou knows who you are when you write, without searching | Encrypted; how you relate to the owner, how close you are, and relationships between people come only from the owner, never guessed; never sensitive information; erased with your data on request |
| The organisation you write from, found from the domain of your email address (never a free mailbox like Gmail), your role there if the owner says so, and the topics you discuss with the owner once they come up in more than one conversation | So a new message comes with its history, even from another address of the same organisation | Encrypted; domains stored as keyed fingerprints, never in clear; never sensitive information; your link to an organisation is erased with your data on request |
| The owner's preferences about dealing with you (for example "always in French") | So Lou follows how the owner likes things | Encrypted; only from the owner, never from your messages; they can never give Lou a permission; erased with your data on request |
| A log of every change to what Lou knows (what changed, from where, by whom) | So each change can be explained and undone | Encrypted; can't be rewritten; its content is erased after 12 months, or with your data on request |
| Short facts Lou learns, about you or the owner (where you work, a preference, a plan), each with where it came from; and what was to do between you and the owner, and how it ended | So Lou remembers what matters and doesn't raise the same thing twice | Encrypted; never sensitive information; facts learned from your messages are listed to the owner, who can correct or remove them; erased after 12 months, or with your data on request |
| A search index of what Lou keeps: fingerprints of words, and "meaning" vectors | So the owner can find anything by asking ("what did Clara say about the deck?") | Built only from text with sensitive details removed; words stored as keyed fingerprints, never as words; vectors encrypted; nothing from people who opted out; erased with the content |
| Messages Lou drafted, whether the owner approved them, and whether they were sent | Accountability: every message has a record | Encrypted, with a tamper-evident fingerprint |
| An activity log: what happened and when (ids, times, statuses, costs) | Audits: anything Lou did can be traced | **Contains no message content.** Cannot be altered or deleted, even by Lou |

**Never kept:**
- notes or profiles containing sensitive information about you: health, political opinions, religion, sexual orientation, ethnic origin, legal
  trouble, relationship crises, and similar (Lou's case files are written only from checked messages, and checked again when the rules grow);
- **sensitive details in your messages**: an automatic check, run in the European Union, removes them **as soon as a message arrives, before
  anything else in Lou can read it** ("can't make it tomorrow, [personal reason]"), and erases them from the copy that is stored. Until the check
  has passed a message, no part of Lou can read it; when the check can't run, the message waits, unread, and is checked again later. This
  includes **money trouble**, the owner's too (an overdraft, a debt, a loss, a collection) and bank or card numbers, replaced by
  "[financial detail]"; a price or an amount to pay or reimburse is not sensitive and stays;
- voice recordings, once transcribed;
- anything from people who chose the **no content** or **ignore** level (see below): their messages are dropped before they are stored.

## Where it is kept, and who else sees it

- **Storage:** on servers located in the **European Union**, and on the owner's own devices. Content is encrypted with keys held by the owner;
  the hosting provider cannot read it.
- **AI providers**, only for the excerpt needed for a given task, never your whole history:
  - **Mistral**, based in the **European Union**, runs the privacy check: it is the filter between the world and the rest of Lou. It receives
    only the messages a first set of rules flags. It also makes Lou's search understand meaning ("the apartment" also finds "the flat");
    later, speech-to-text.
  - **Anthropic** (Claude), a company based in the **United States**, prepares answers and drafts, and keeps the case files (where things
    stand with each person or organisation, what is open, each point with its messages). It reads messages **only once the privacy check
    has passed them**, never before. Under its commercial terms, this data is not used to train its models.
- **Web searches:** for public, current information (a train's status, a company, a place), Lou can search the web through its AI provider.
  Searches are about public things: Lou is instructed never to put your name or details in one, and every search is recorded so the owner can check.
- **The platforms the messages already go through:** WhatsApp (Meta) for Lou's own number, and Google for the owner's email and calendar,
  accessed through their official interfaces with the owner's permission.

Nothing is sold or shared for advertising. Nothing is published.

## How long

- Messages, emails, drafts and the owner's chats with Lou: their **text is erased automatically after 12 months**, or earlier if you ask.
  What remains is a record without content (who wrote, when, whether a message was sent, and a fingerprint that proves what was sent
  without allowing anyone to read it again), kept with the activity log.
- Case files and the log of changes to what Lou knows: their text is erased after 12 months too.
- Voice recordings: deleted once transcribed.
- The activity log: kept **3 years**, because it is what makes Lou auditable. It holds no message content.
- Backups: a weekly encrypted copy of Lou's database, on the owner's own devices; the last **8 weeks** are kept. Something erased
  (on request or after 12 months) disappears from the backups as they're replaced, within 8 weeks. Backups are only used to restore
  Lou after a failure.

## Messages Lou sends

Lou writes to someone only when the owner asked for that message and approved the exact text. Each message is signed **"Lou"** (the first one links
here), unless it is the owner's own words. You can ask how any message was written: see the [Lou card](lou-card.en.md).

Lou can also prepare a message that the owner then sends **from their own phone, as their own message**; by default, for people close to the
owner. Such a message isn't signed Lou, because the owner sends it; how it was written (and by how much Lou) is recorded all the same, and you can
ask about any message you received from the owner.

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

**How to ask:** write to **lou.kernel@gmail.com**, reply to any message signed Lou, or tell the owner directly. If you ask the owner in a message not to be contacted by Lou or not to have an AI read your messages, Lou registers
it as a request and tells the owner at once. The owner handles each request personally: opt-outs immediately, other
requests within 30 days. Each request is registered with its deadline and followed until it is answered. An erasure is prepared by Lou
and runs only once the owner has approved it; it removes the text of your messages, your name and your contact details, and keeps only a
record that messages existed and when, with your contact details as unreadable fingerprints so that your choices keep applying. Wherever the
owner or Lou wrote your name or contact details (the owner's own messages to Lou, reminders, to-dos, Lou's logs), they are replaced by
"[erased]": the records stay, without you in them.

If you live in the EU, you also have the rights given by the GDPR, including complaining to your data protection authority.

## Security

Content encrypted at rest; a separate component, holding no AI access, is the only one able to send anything, and only messages the owner approved
(checked by a cryptographic signature); every step is recorded in a log that cannot be changed. Details of the infrastructure are deliberately not
published.

## Changes

This policy changes when Lou changes. Each version is listed in the [changelog](CHANGELOG.md), with what changed and why.
