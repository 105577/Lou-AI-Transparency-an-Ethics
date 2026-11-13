# Changelog

## 0.2.13 · 2026-11-13
- One check at arrival: the privacy check, run in the EU, now passes every message as soon as it arrives, before any other part of Lou
  can read it. Until it has, no part of Lou reads the message; if the check can't run, the message waits, unread, and is checked again.
  Money is sensitive when it is trouble (an overdraft, a debt, a loss) or an account number, not when it is a price or an amount to
  reimburse.
- Which AI reads what: Mistral (EU) is the filter between the world and the rest of Lou. Lou's main AI (Anthropic's Claude) now also
  keeps a case file per person and organisation: where things stand and what is still open, each point with the messages that prove it.
  It reads only what the filter has passed, and code refuses any point that no message proves. This replaces the short note per
  conversation and the daily AI review.
- Lou asks rather than guesses: when something may have been settled out of its sight (a call, a meeting), it asks the owner in one
  line. It now knows when the owner called someone it already knows, from the owner's own computer: who, when and how long, never what
  was said.
- Names: two records with the same full name are treated as one person, and the owner can separate them. The owner can give Lou their
  contacts as a file, to put names on numbers; Lou adds nobody from it.
- Who sends a draft: the owner can send a message Lou drafted from their own phone, as their own (by default, for people close to them).
  It isn't signed Lou; how it was written is recorded all the same, and you can ask about any message.
- Erasure goes further: wherever the owner or Lou wrote your name or contact details (the owner's messages to Lou, reminders, to-dos,
  Lou's logs), they are replaced by "[erased]". The log of changes to what Lou knows now also loses its text after 12 months, like the
  rest; every encrypted field now states its retention and erasure, checked automatically.
- How Lou learns: from the owner's words (what's done, what to drop, a correction), from what became of each draft (sent as is, edited,
  not sent) and from what the owner does with each heads-up. Its rules change only through reviewed code.

## 0.2.12 · 2026-11-09
- Backups: once a week, Lou makes an encrypted copy of its database, kept on the owner's own devices, so a failure or a mistake can't
  wipe what Lou knows. The last 8 copies are kept (about two months). They're encrypted before they're written, with a key only the
  owner holds, and the status warns the owner if no backup was made for more than 8 days.
- What this means for erasure: when you ask for your data to be erased, it's erased from Lou at once, and it disappears from the
  backups as they're replaced, within 8 weeks at most. A backup is only ever used to restore Lou after a failure.
- Heads-ups are steadier: dates, and whether the owner has to act, are checked by code rather than left to the AI's wording.

## 0.2.11 · 2026-11-09
- Heads-ups, rethought: Lou now reads each conversation once, when it has moved and gone quiet, instead of each message on its own. One
  call to the small AI model in the EU writes the conversation's note and says what it asks of the owner, by when and how much is at
  stake. Whether to tell the owner now or in the morning brief is then decided by code, with rules that can be read, not by a second AI.
- To judge well, that call now also sees the owner's calendar for the next 7 days and their free slots, past matters with the person,
  and upcoming birthdays. It still never receives sensitive details, and plain thanks, newsletters, calendar replies and muted chats
  never reach any AI.
- If you write to the owner that you don't want to be contacted by Lou, or don't want an AI to read your messages, Lou registers it as
  a request and tells the owner at once, so it doesn't depend on someone noticing.
- What the owner promises in their own messages ("I'll send it tomorrow") is kept as a to-do for them.
- The daily review also writes the morning brief, in the same run, so one AI pass a day instead of two.

## 0.2.10 · 2026-11-08
- Organisations and topics: Lou groups what it knows by organisation, recognised by the domain of its email addresses (never a free
  mailbox like Gmail), and by topic, once it comes up in more than one conversation. A new email, even from another address of the same
  organisation, comes with its history: what was raised before and what the owner did about it.
- Preferences: the owner can tell Lou how they like things (style, priorities), everywhere or for one person, organisation or topic. A
  preference can never give Lou a permission: approvals, who Lou may contact, privacy and limits change only in Lou's code, reviewed,
  and Lou refuses such requests whoever makes them. Preferences come only from the owner, never from anyone else's messages.
- One log of every change to what Lou knows, encrypted and impossible to rewrite, so each change can be explained and undone.

## 0.2.9 · 2026-11-08
- Contact cards: Lou keeps a short card per person (name, birthday, how they relate to the owner, the latest context) so it knows who
  is writing without searching. Relationships and closeness come only from the owner, never guessed; nothing sensitive; erased on request.
- Lou asks the owner when it lacks context (who someone is, what a meeting is about), a few questions a day at most.
- Once a day, Lou looks over the owner's open threads to catch what could be forgotten (a reply still awaited, a birthday coming), with
  read-only access: it can't send or change anything in that review. Heads-ups are rarer: only what the owner would thank Lou for.

## 0.2.8 · 2026-11-08
- Search: the owner can find anything Lou keeps by asking, by words or by meaning. The index is built only from text with sensitive
  details removed: words are stored as keyed fingerprints (never as words), and "meaning" vectors, made by a small model in the EU,
  are stored encrypted. Nothing from people who opted out is indexed, and the index is erased with the content.
- Knowledge: Lou keeps short facts it learns (about people and the owner), each with its source and never sensitive, and follows what
  it raised with the owner like a case, from raised to closed with the owner's reason, so it doesn't raise the same thing twice. Facts
  learned from someone's messages are shown to the owner, who can correct or remove them; they're erased after 12 months, or on request.
- Events: Lou now keeps an event's description (with sensitive details removed when read), its video link and who is invited, so it
  can help the owner prepare a meeting.

## 0.2.7 · 2026-11-04
- Money details are now filtered like other sensitive information, the owner's included: account balances, amounts, bank or card numbers,
  IBAN and salary are removed before Lou's AI reads a message and erased from what is stored, keeping only what is asked and by when.
  What was already stored has been checked again.

## 0.2.6 · 2026-11-04
- Living notes: Lou keeps a short note per conversation (where things stand, what each side still owes) so the owner doesn't have to re-read
  everything, and offers help when it can. Notes are written from messages with sensitive details already removed, checked again, never
  carry instructions from anyone's message, can be corrected by the owner, and are erased with the messages (12 months, or on request).

## 0.2.5 · 2026-11-04
- Heads-ups: when someone asks for the owner's availability, agrees a time, sends an invitation or a deadline, Lou tells the owner (a few
  times a day at most, never at night) and offers to prepare the answer, which the owner still approves. To understand what a message asks,
  Lou uses a small AI model in the EU, on the message with sensitive details already removed.

## 0.2.4 · 2026-11-04
- Requests about your data (see, correct, erase, opt out) are registered with their deadline and followed until answered. An erasure is
  prepared by Lou and runs only after the owner approves it; a record without content proves it was done.

## 0.2.3 · 2026-11-04
- Retention: the text of messages, emails, drafts and the owner's chats with Lou is erased automatically after 12 months. A record without
  content stays with the activity log, which is kept 3 years.

## 0.2.2 · 2026-11-04
- Lou can search the web for public information (a train's status, a company, a place). Searches never contain anyone's personal details by rule,
  and each one is recorded.
- Sensitive details about others (health, beliefs, family matters…) are removed automatically before Lou's AI reads any message, and erased
  from what is stored, including Lou's own replies. The check runs in the EU; when it can't run, the message is hidden from Lou instead.
- The owner can set privacy levels for someone, or tell Lou never to read emails from a domain (for example a medical office): applied before anything is stored.

## 0.2.1 · 2026-11-02
- Email: Lou now keeps the text of the owner's emails (encrypted), not only the subject and a short preview, so replies answer what was actually
  written. Attachments are never opened. People who opted out (no content, ignore) are unaffected: nothing of theirs is kept.
- Autonomy: changes to the owner's own calendar that the owner asked for, on events with nobody else on them, are applied directly and confirmed
  (level A3). Everything that reaches another person is still approved word for word; deleting an event or changing one with guests still needs approval.

## 0.2.0 · 2026-11-02
- Lou is in early use by its owner. It reads the owner's messages (read-only), email (sender, subject and short preview, never the full body) and calendar.
- Lou can now send messages and emails for its owner, **only after the owner approves the exact text**, each one signed (cryptographically checked in code).
- Contact address published: lou.kernel@gmail.com (Lou's own address; the owner answers personally).
- New: privacy policy (EN/FR): what Lou reads and keeps, where, how long, who else sees it, and how to limit or erase it.
- Lou card: clarified that the "never kept" rule covers Lou's notes about people (no notes are written until the sensitive-information filter is live);
  sealing marked as in progress.

## 0.1.1 · 2026-10-28
- Principle 8: on any misuse attempt, Lou cuts itself out of the conversation and stays off until its owner has reviewed the case.
- Lou card: Lou keeps no copy of voice recordings once transcribed.

## 0.1.0 · 2026-10-28
- First publication: About Lou (EN/FR), principles (EN/FR), Lou card (EN/FR).
- Lou card: three opt-out levels (no contact, no content, ignore), checked in code before any AI.
- Lou is in development and not live yet. All actions require the owner's approval.
