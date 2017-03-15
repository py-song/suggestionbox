# suggestionbox
Slack integration/bot for a suggestion box system

Specs:
======

General:
------
- slash command: `/suggest suggestion goes here`
- public channel: _#suggestionbox_
- bot user: `@suggestionbot`

Install:
------
- on install, creates channel, bot joins and invites all team users
- posts new welcome post for `@channel`, pins it to channel
- posts suggestion number 0 as an example

Usage:
------
- `/suggest new suggestion` -> posts new suggestion in channel with a number
- `@suggestionbot` will DM you that your suggestion has been posted along with its number
- users can reply in thread to talk about specific topic

Additional features:
------
- restrict top level posting in channel
- anonymous threaded replies leveraging the fact that each suggestion is numbered: `/suggest 4 reply to suggestion`
- store suggestions somewhere -> google keep webhook?
- track suggestion issuers -> intended to track inappropriate usage due to anonymity
- limit slash command to channel only
