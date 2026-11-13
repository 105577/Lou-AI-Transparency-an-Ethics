# Lou card

**Version 0.2.13 · 2026-11-13 · Status: in early use by its owner.** Lou reads its owner's messages, email and calendar, and sends messages and emails only after its owner approves each one.

## Purpose & limits
A personal assistant: it tracks commitments, prepares replies and meetings, and keeps context about its owner's plans and network.
It does **not** act on its own, commit its owner to money, legal matters or agreements, or interact with people who opted out. Full list: [principles](principles.en.md).

## Autonomy
Today **every message or action that reaches another person is approved by its owner**, word for word, before it happens.
The only exception concerns the owner alone: changes to the owner's own calendar that the owner asked for, on events with nobody else on them,
are applied directly and confirmed (level A3 below). Any change to this is announced in the [changelog](CHANGELOG.md).

## Models & data
| Role | Provider |
|------|----------|
| Privacy check at arrival: removes sensitive details before any other part of Lou can read a message; search by meaning; later speech-to-text | Mistral (EU) |
| Conversation, drafting, and the case files (where things stand with each person or organisation, what is open, each point with its messages), only from messages the privacy check has passed | Anthropic (Claude) |

Data is stored on servers in the EU and on the owner's own devices. AI providers receive only the excerpts needed for a given task.

## Data practices
- Never kept: notes or profiles with sensitive information about others (health, political opinions, religion, sexual orientation, ethnic origin, etc.). Lou keeps a case file per person or organisation (where things stand, what is open), written only from checked messages; a point that no message proves is refused by code.
- One gate at arrival: sensitive details about others are removed as soon as a message arrives, and erased from what is stored; until then, no part of Lou can read it. Money trouble and bank or card numbers are treated the same way, the owner's included; a price or an amount to reimburse stays.
- Phone calls: Lou knows when the owner called someone it already knows, and for how long, never what was said.
- Erasure: what you wrote goes, and your name and contact details are replaced by "[erased]" wherever the owner or Lou wrote them.
- A weekly encrypted backup of Lou's database is kept on the owner's devices for 8 weeks; erased data leaves the backups within that time.
- Lou keeps a short contact card per person (name, birthday, how they relate to the owner, the latest context). How people relate to the owner and to each other comes only from the owner, never guessed.
- Lou also groups what it knows by organisation (from email domains) and by recurring topic. The owner's preferences shape style and priorities only: they can never give Lou a permission.
- Possibly sensitive content is sealed: encrypted with a key only the owner holds, so Lou itself can't read it *(in progress)*.
- Full details: [privacy policy](privacy-policy.en.md).
- Lou keeps no copy of voice recordings once they are transcribed.
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
| G2 | Enhanced by Lou from the owner's text | A3 | Done by Lou under a standing permission (only the owner's own calendar, at their request) |
| G3 | Generated from detailed instructions | | |
| G4 | Generated from a short instruction | | |
| G5 | Generated without a specific instruction | | |

Messages at G2 and above are signed "Lou". G0–G1 messages are signed by the owner.
A draft the owner sends from their own phone is their own message and isn't signed Lou (by default, for people close to the owner); its
generation record is kept all the same, and available on request.

## Contact
**lou.kernel@gmail.com** (the owner answers personally).
