# Gobble Gobble Go!

A family-friendly Thanksgiving party game that runs in a phone's web browser. Two teams take turns: the clue giver gets a card and has to get their team to guess it before the timer runs out.

Clue types:

- **Act it out**: no talking, no sounds
- **Describe it**: talk, but don't say the word
- **Gobble only**: the only word allowed is "gobble"
- **Pictionary**: draw it on the screen
- **Gobble the song**: sing a pop hit (1950s to today) using only "gobble"
- **Gobble the movie line**: act out a famous movie quote saying only "gobble"

## Ways to play

- **Solo / local**: pass one phone around the room.
- **Online (up to 10 players)**: everyone plays on their own phone. Create a room, share the 4-letter code or the `?room=CODE` link, and the host starts the game. Only the clue giver sees the clue. Clue givers rotate at random, and nobody repeats until everyone on their team has had a turn. Players who drop can rejoin with the same code.

Online play is peer-to-peer through [Trystero](https://github.com/dmotz/trystero) (MQTT, with Nostr as the fallback), so there's no server to run.

## Run it

It's one file, `index.html`, with no build step. To put it online with GitHub Pages:

1. Go to **Settings → Pages** in this repository.
2. Under **Build and deployment**, choose **Deploy from a branch**, then pick `main` and `/ (root)`.
3. Save. The game will be at `https://bberlin722.github.io/Gobble-Google-Go/`.

Online play needs the page served over `https://` (GitHub Pages does this). Opening the file straight from your computer only works for solo play.
