# plot-armor-games-data

The game lists for **Plot Armor: Gaming**, a Chrome extension that covers video game story
spoilers on X. Published with GitHub Pages at
https://sellybros711.github.io/plot-armor-games-data/

- One JSON file per game (names, characters, places, keywords, release date). The format is
  described in the extension's CLAUDE.md ("Game JSON format").
- `index.json` lists the files: `{ "games": ["gta-6.json", ...] }`. A new game needs its file
  AND its name in that list.
- The extension downloads these once a day and checks every file before using it. A file with
  a mistake is ignored and users keep the last good copy.
- `privacy.html` is the extension's privacy policy.

Edit the files in `~/Projects/plot-armor-games/src/data/games/` first, run `npm test` there,
then copy them here and push.
