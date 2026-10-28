# Lou card

**Version 0.1.0 · 2026-10-28 · Status: in development, not live yet.**

## Purpose & limits
A personal assistant: it tracks commitments, prepares replies and meetings, and keeps context about its owner's plans and network.
It does **not** act on its own, commit its owner to money, legal matters or agreements, or interact with people who opted out. Full list: [principles](principles.en.md).

## Autonomy
Today **every outgoing message or action is approved by its owner** before it happens. Any future change to this is announced in the [changelog](CHANGELOG.md).

## Models & data
| Role | Provider |
|------|----------|
| Conversation, drafting, planning | Anthropic (Claude) |
| Speech-to-text, search indexing, small classification tasks | Mistral |

Data is stored on servers in the EU and on the owner's own devices. AI providers receive only the excerpts needed for a given task.

## Data practices
- Never stored: sensitive information about others (health, political opinions, religion, sexual orientation, ethnic origin, etc.).
- Possibly sensitive content is sealed: encrypted with a key only the owner holds, so Lou itself can't read it.
- Voice recordings are deleted within 24 hours of transcription.
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
| G2 | Enhanced by Lou from the owner's text | A3 | Sent by Lou under a standing permission (not used today) |
| G3 | Generated from detailed instructions | | |
| G4 | Generated from a short instruction | | |
| G5 | Generated without a specific instruction | | |

Messages at G2 and above are signed "Lou". G0–G1 messages are signed by the owner.

## Contact
**lou@…** (the owner answers personally).
