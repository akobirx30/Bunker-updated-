# Bunker (online card game)

A browser version of the party game Bunker: each player gets a secret dossier, reveals cards round by round, and the group votes who gets expelled until only the bunker's spots are left.

- 3 to 8 players, each on their own phone, joined by a 4-letter room code
- Card set: 50 professions, 32 biology, 32 health, 32 hobbies, 50 facts, 32 baggage, 32 special conditions, 10 catastrophes, 21 threats, 30 bunker cards
- All card names, texts and icons are original; icons are emoji drawn as silhouettes

## Important

`index.html` uses the `room` capability of the Claude artifact runtime (`claude.use("room")`) for real-time play.
That API only exists inside a published Claude artifact, so **multiplayer does not work when this file is opened from GitHub Pages or locally**.
To host it on its own, replace the room layer (the `enter`, `send` and `R.*` calls) with a service such as PeerJS or Firebase.
