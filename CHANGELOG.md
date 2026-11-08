# Changelog

## 0.2.8 · 2026-11-08
- Search: the owner can find anything Lou keeps by asking, by words or by meaning. The index is built only from text with sensitive
  details removed: words are stored as keyed fingerprints (never as words), and "meaning" vectors, made by a small model in the EU,
  are stored encrypted. Nothing from people who opted out is indexed, and the index is erased with the content.
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
