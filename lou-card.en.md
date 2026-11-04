# Lou card

**Version 0.2.6 · 2026-11-04 · Status: in early use by its owner.** Lou reads its owner's messages, email and calendar, and sends messages and emails only after its owner approves each one.

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
| Conversation, drafting, planning | Anthropic (Claude) |
| Privacy check on messages (removes sensitive details), understanding what a message asks (for heads-ups); later speech-to-text | Mistral |

Data is stored on servers in the EU and on the owner's own devices. AI providers receive only the excerpts needed for a given task.

## Data practices
- Never kept: notes or profiles with sensitive information about others (health, political opinions, religion, sexual orientation, ethnic origin, etc.). Lou keeps a short note per conversation (where things stand, what's pending), written from messages with sensitive details already removed and checked again.
- Sensitive details about others are removed automatically before Lou's AI reads any message, and erased from what is stored.
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

## Contact
**lou.kernel@gmail.com** (the owner answers personally).
