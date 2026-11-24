# Changelog

## 0.2.27 · 2026-11-24
- **Groups are read**, like the owner's other conversations: a dinner agreed in a group was missed because Lou only read a group for a
  few days after the owner wrote there. Not read: groups the owner set to never read, and groups the owner muted or archived in their
  app, unless a message names the owner. The privacy policy says so in its group line.
- **Lou's own agenda**, beside the owner's calendar and never added to it: a reminder or a question for the owner, sent once at a
  time, the next time the owner is with someone ("ask Paul whether he can drive"), or before or after a meeting; and where the owner
  will be, from their own words. Its text is deleted after 12 months, and an erasure reaches it like the rest.
- **The bridge** (notes from the owner's other assistant, accepted only from the owner's own Sent mail): such a note is now handled as
  a message from the owner, under the same rules: anything that would go to someone still waits for the owner's "send". These notes
  had been dropped by mistake since the start; nothing else was affected.
- One person on several apps is one person again: records with the same full name, or the same phone number on two apps, are linked
  every hour. The owner can always separate two people Lou linked.
- A meeting that was moved or updated is no longer reported to the owner as clashing with itself.
- Lou tells the owner when it hasn't been able to update itself for 20 minutes, with what to do.

## 0.2.26 · 2026-11-24
- A booking from a company's email (a train, a flight) goes into the owner's calendar only when the owner's email provider confirmed
  the email really comes from that company's address. An email that only pretends to be from a company adds nothing.
- When a company's email gives a train's number and its departure time but not its arrival, Lou finds the arrival in the public
  timetable, still searched on the owner's devices.

## 0.2.25 · 2026-11-24
- The owner's calendar, done by Lou: a meeting agreed in a conversation now goes into the owner's calendar by itself (it was in a test
  mode). A dinner agreed for a day with no time blocks the evening; a lunch, the middle of the day.
- A train booked without its times in the email: Lou finds them in SNCF's public timetable. Lou downloads the whole timetable and
  searches it on the owner's devices, so no one learns which train the owner takes. If several trains fit, Lou asks the owner.
- If you give the owner your phone number or email address in a message, Lou adds it to how it recognises you. Never a number
  someone else gives about you, and a number from a message never makes two people one: if Lou already knows it as someone else's,
  it is left alone.
- Something to bring to a meeting ("bring an ID") becomes a reminder for the owner before leaving.
- Groups are read for 7 days after the owner writes in them (it was 48 hours), so a question asked a few days later is not missed.
  The owner's own reply in a group is linked to the person they answered.
- A to-do that needs someone ("ask Paul") is said to the owner when they are together, from the owner's own message or a meeting
  with them. Lou keeps only that link (who, when), never your words.
- The owner can teach Lou how to do a kind of task, in their own words; Lou follows it from then on. Never from what other people
  write: Lou doesn't keep one in an answer where it read someone else's message. Twice a day, Lou names questions
  the owner hasn't answered yet; and when someone proposes a time, Lou tells the owner whether they're free and offers a reply. Any
  reply still needs the owner's *send*.

## 0.2.24 · 2026-11-23
- Bookings in the calendar again: a train or a flight the owner books (from the company's own email) goes into the owner's calendar, one
  block per leg, as 0.2.13 said. Since 0.2.16 it no longer did; this fixes it. Never from someone else's message about their trip.
- LinkedIn, for the owner's job search: once a week the owner's assistant (Claude, in the owner's own browser) lists whom the owner
  invited and who accepted, and sends it to Lou. Lou keeps each name with the headline and company LinkedIn shows, never as a new
  person, and nothing for someone who asked not to be read. Nothing reads LinkedIn automatically from Lou's side.

## 0.2.23 · 2026-11-23
- The owner's app was rebuilt: what Lou is doing (what it read, what it skipped and why, what it cost), who is under a restriction,
  and how each group is read, all managed in one place. Each change still needs the owner's passkey, is logged, and follows the same
  rules as before: an opt-out you asked for yourself can only be lifted by you.
- Groups: the owner can set each group to be read always, only while the owner takes part (the default: 48 hours after the owner
  writes in it or is named), or never. A group set to never read gives Lou no notes (no to-dos, no times); its messages stay stored
  and searchable. The privacy policy now says how groups are read, in its own line.

## 0.2.22 · 2026-11-21
- A review of the last two days' changes found an error and four weaknesses, all fixed the same day:
  - **The error:** an opt-out you asked for yourself could be undone by the owner in two steps (first a stricter setting, then a lift).
    Now your own choice is always what counts: only you can lift it.
  - **The bridge:** notes from the owner's other assistant are accepted only from the owner's own Sent mail, never from an email that
    merely shows the owner's address as its sender (that can be forged).
  - **Learning:** what Lou learns can't carry someone else's words: it never reads what Lou drafted or searched from other people's
    messages, and a procedure with an email address, a link or someone's name is refused.
  - **The owner's past sent emails:** none written to someone who opted out is read, forwarded emails are cut, and none is kept as an
    example.
  - **Travel times:** a place that is someone's home ("chez …") is never sent to the address service.

## 0.2.21 · 2026-11-21
- Lou learns how to do things, like an assistant who gets better with practice: after a task that took several steps, or one the owner
  corrected, it writes a short procedure for that kind of task (when it applies, its steps, an example) and refines it after the owner's
  next correction. It learns only from the owner's messages, its own steps and the owner's corrections, never from what other people
  write. A procedure can't change a permission, a privacy setting or a budget, and anything that goes to someone still needs the
  owner's *send*. The owner sees each one, with its versions, and can retire it. Written in a test mode first, not yet followed.
- The owner's other AI assistant (Claude, in the owner's own sessions) can send Lou notes by email, from the owner's own address. Lou
  files them as notes about the owner, never as instructions: nothing in them can make Lou contact anyone. A note that might carry a
  sensitive detail is left out.
- One question a day at most: when a missing fact stops Lou from doing something (a meeting agreed with no time can't go in the
  calendar), Lou asks the owner once. Never about a fact Lou can do without.

## 0.2.20 · 2026-11-21
- The owner manages Lou from an app (the dashboard, on the owner's private network, unlocked with their passkey): closing or
  reopening a to-do, dropping a meeting that went nowhere, how Lou treats someone, adding an email address, what Lou remembers about
  the owner. Each change is logged and follows the same rules as when the owner tells Lou: an opt-out you asked for yourself can only be
  lifted by you.
- The owner's corrections: the owner can mark one of Lou's answers as wrong and say what Lou should have done. The words are encrypted,
  erased after 12 months, and all of them at any erasure request.
- The owner's LinkedIn connections file: for people Lou already knows (matched by email address), their company and position. As with
  the owner's contacts file, nobody new is added, and nothing is added for someone who opted out.

## 0.2.19 · 2026-11-21
- Real travel times: around an in-person meeting, the time to get there by public transport instead of a fixed 45 minutes, from
  Île-de-France Mobilités, with addresses placed by the national address service (IGN). Only the two places of the trip are sent,
  never who the meeting is with. When the service can't answer, the 45 minutes stay.
- How the owner writes emails: once, Lou reads the owner's own words in past sent emails (up to 400, the last 3 years; quoted
  messages cut, recipients not kept), each through the privacy check first, to learn the owner's email style. The emails are deleted
  within days, once read; only the style description and a few examples stay, as in 0.2.18.

## 0.2.18 · 2026-11-21
- Drafts that sound like the owner, even to someone new: from the owner's own messages (only those the privacy check has passed), Lou
  keeps a short description of how they write, per language and kind of relationship (family, friends, recruiters, work…): tu or
  vous, length, greetings, usual turns of phrase. Style only, naming nobody. Up to three of the owner's own messages are kept, as
  written, as examples; they are erased after 12 months, and all of them at any erasure request.

## 0.2.17 · 2026-11-21
- One reading of each message: once the privacy check has passed a message, Lou reads it once, with the few before it in that
  conversation, to note what is to do, who owes what, and times proposed, accepted or cancelled. Each note must quote the message it
  comes from. Code refuses a note no message proves, someone else closing one of the owner's own to-dos, and anything about where the
  owner will be that doesn't come from the owner. Facts about people are not kept from this reading yet: they are measured first.
  Nothing in it can send, pay, share or delete.
- Before any AI, rules leave out what isn't worth reading: automated mail other than bookings, very short messages, and groups the owner
  neither takes part in, nor is named in, nor turned on. People who chose *no content* or *ignore* are never read. Each decision is
  logged with its rule's name, so a message left out can always be explained. At night this reading waits for the morning, except in a
  conversation where a time is being agreed.
- Answering the owner: a smaller Claude model now answers; the main one still writes anything that goes to someone else. Before the
  switch, the owner's recent questions were replayed through it, with nothing sent or changed, and the answers compared with the ones
  given at the time, by the reviewer the owner allowed. Those replayed answers are kept encrypted for 12 months.
- Lou does what its tools can do and then says what it did, instead of asking first. Sending anything on the owner's behalf still needs
  exactly the word *send*.

## 0.2.16 · 2026-11-20
- Lou does less in the background, on purpose, while its understanding is rebuilt: no more case files, morning brief, heads-ups, project
  proposals or after-meeting questions. Reminders, meeting reminders, the privacy check, search and the owner's calendar work as before.
  Someone asking not to be contacted or read by an AI is still reported to the owner at once.
- Spending limits on every AI call: a cap per day, and at night (00:00 to 07:00) background work waits for the morning.
- Sending something on the owner's behalf now needs exactly the word *send* (or *no* to drop it), checked by code: no other phrasing, no
  emoji, and with several drafts waiting, only the one the owner replies to.
- A reviewer, with the owner's consent: the owner can let a reviewer (an AI assistant working for the owner) read Lou's logs for a few days
  at most, revocable at any time; it sees only what passed the privacy check, with phone numbers and email addresses masked, and every
  reading is recorded.

## 0.2.15 · 2026-11-17
- The owner's calendar follows their words: when the owner's own message moves or cancels a time Lou blocked, Lou moves or removes the
  block and says so, with a one-word undo. Someone else's message alone still changes nothing. Undo now also puts back a move or a removal.
- What the owner says in a group that they'll do ("I'll bring the drinks") becomes one of their to-dos, with that message as its proof.
- Heads-ups no longer adjust themselves from the owner's reactions: only the owner's own settings ("fewer", "more", "never") change them.
  This replaces what 0.2.13 said about learning "from what the owner does with each heads-up"; Lou still learns from the owner's words and
  from what became of each draft.

## 0.2.14 · 2026-11-17
- Voice notes: the owner can talk to Lou. Their voice notes are turned into text in the EU (Mistral) and the audio is deleted once heard.
- What the owner sends Lou: images and PDFs (a ticket, a screenshot of a booking) are read in the EU (Mistral) and deleted once read, a day
  at most; only the text is kept. Anything that isn't the owner's own voice, a forwarded message included, passes the privacy check before any
  other AI reads it (forwarded text messages didn't before: now they do).
- Web pages: besides searching the web, Lou can read a public page, only one whose address is already in the conversation, so it can't build
  an address with your details. Every page read is recorded, like every search.
- What Lou can do is now declared in one place in its code, and the list on the Lou card is generated from it: a capability that isn't
  declared, with where its data goes and its own monthly budget, can't ship.

## 0.2.13 · 2026-11-17
- The owner's own calendar: when the owner agrees to a time in their own words (in a chat, a group or an email), Lou blocks it on their
  calendar within a minute and tells them, with a one-word undo; a booking an organisation sends (a train, a hotel) too. To notice it, Lou's
  main AI reads the owner's message with the few before it in that conversation, only once the privacy check has passed them. A message
  from someone else alone never changes the owner's calendar: at most, Lou suggests it to the owner.
- Who said what: in an email, the earlier messages it quotes are no longer read as its sender's own words.
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
