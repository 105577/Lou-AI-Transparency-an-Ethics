# Lou card

**Version 0.2.19 · 2026-11-21 · Status: in early use by its owner.** Lou reads its owner's messages, email and calendar, and sends messages and emails only after its owner approves each one.

## Purpose & limits
A personal assistant: it tracks commitments, prepares replies and meetings, and keeps context about its owner's plans and network.
It does **not** act on its own, commit its owner to money, legal matters or agreements, or interact with people who opted out. Full list: [principles](principles.en.md).

## Autonomy
Today **every message or action that reaches another person is approved by its owner**, word for word, before it happens.
The only exception concerns the owner alone: their own calendar, on events with nobody else on them. Lou adds or moves an event when the
owner asks, and blocks on its own a time the owner agreed to in their own words, or a booking an organisation sent (a train, a hotel); when
the owner's own words later move or cancel that time, it moves or removes its block. Each change is said at once in one line, and one word ("undo") takes it back (level A3 below). A message from someone else is never enough to change anything. Any
change to this is announced in the [changelog](CHANGELOG.md).

## What Lou can do
Generated from Lou's capability registry: nothing ships without a line here.
- Answers the owner and prepares drafts (Anthropic, Claude: a smaller model answers, the main one writes what goes to someone else).
- Reads each message once the privacy check has passed it, to note to-dos, who owes what and times proposed or agreed, each with the message that proves it; where the owner will be comes only from their own words, calendar and bookings (Anthropic, Claude). Case files and projects are paused while Lou's understanding is rebuilt.
- Works out travel time to an in-person meeting by public transport (Île-de-France Mobilités and the national address service, IGN); only the two places of the trip are sent, never who the meeting is with.
- Checks every message for sensitive details before anything else reads it, and makes search understand meaning (Mistral, EU).
- Turns the owner's voice notes into text (Mistral, EU); the audio is deleted once heard.
- Reads the text of images and PDFs the owner sends it (Mistral, EU), checked for sensitive details before anything else reads it; the file is deleted once read.
- Searches the web and reads public pages for current information (a train's status, opening hours), through Anthropic; never with your name or details, and every search and page is logged.
- Sends a message or an email only after the owner approves that exact text.
- Adds or moves events with nobody else on them in the owner's own calendar, blocks a time the owner agreed to or a booking, and moves or removes its own blocks when the owner's words change them; each with a one-word undo.

Not built: acting on websites, sending in group chats, inviting people to events.

## Models & data
| Role | Provider |
|------|----------|
| Privacy check at arrival: removes sensitive details before any other part of Lou can read a message; search by meaning; the owner's voice notes to text, and the text of images and PDFs the owner sends | Mistral (EU) |
| Reading each message once for to-dos and times, answering the owner (a smaller model) and drafting (the main one), only from messages the privacy check has passed; web searches and public pages | Anthropic (Claude) |

Data is stored on servers in the EU and on the owner's own devices. AI providers receive only the excerpts needed for a given task.

## Data practices
- Never kept: notes or profiles with sensitive information about others (health, political opinions, religion, sexual orientation, ethnic origin, etc.). The case files Lou wrote until 0.2.15 (where things stand with a person or organisation, what is open) were written only from checked messages; none are written while Lou's understanding is rebuilt.
- One gate at arrival: sensitive details about others are removed as soon as a message arrives, and erased from what is stored; until then, no part of Lou can read it. Money trouble and bank or card numbers are treated the same way, the owner's included; a price or an amount to reimburse stays.
- Phone calls: Lou knows when the owner called someone it already knows, and for how long, never what was said.
- Erasure: what you wrote goes, and your name and contact details are replaced by "[erased]" wherever the owner or Lou wrote them.
- A weekly encrypted backup of Lou's database is kept on the owner's devices for 8 weeks; erased data leaves the backups within that time.
- Lou keeps a short contact card per person (name, birthday, how they relate to the owner, the latest context). How people relate to the owner and to each other comes only from the owner, never guessed.
- Lou also groups what it knows by organisation (from email domains) and by recurring topic. The owner's preferences shape style and priorities only: they can never give Lou a permission.
- Possibly sensitive content is sealed: encrypted with a key only the owner holds, so Lou itself can't read it *(in progress)*.
- Full details: [privacy policy](privacy-policy.en.md).
- What the owner sends Lou: voice notes are turned into text and the audio deleted; images and PDFs are read and deleted (a day at most); only the text is kept. Anything that isn't the owner's own voice (a forwarded message, a screenshot, a document) passes the privacy check before any other AI reads it.
- Everyone is opted in by default and can opt out at any time, at one of three levels:
  - **no contact**: Lou never writes to you;
  - **no content**: Lou only knows that you wrote and when, never what (no AI reads your messages);
  - **ignore**: Lou disregards your messages entirely.
  The check runs in plain code before any AI is involved.

## Generation & agency levels
Each message Lou prepares has a generation record, available on request:

| Generation | | Agency | |
|-----------|--|--------|--|
| G0 | Written by the owner, no AI | A1 | Written and sent by the owner |
| G1 | Corrected or translated by Lou | A2 | Drafted by Lou, reviewed and approved by the owner (current default) |
| G2 | Enhanced by Lou from the owner's text | A3 | Done by Lou under a standing permission (only the owner's own calendar: at their request, a time they agreed to, or a booking) |
| G3 | Generated from detailed instructions | | |
| G4 | Generated from a short instruction | | |
| G5 | Generated without a specific instruction | | |

Messages at G2 and above are signed "Lou". G0–G1 messages are signed by the owner.
A draft the owner sends from their own phone is their own message and isn't signed Lou (by default, for people close to the owner); its
generation record is kept all the same, and available on request.

## Contact
**lou.kernel@gmail.com** (the owner answers personally).
