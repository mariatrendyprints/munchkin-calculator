# Munchkin Calculator — Adventure Time edition

Table-side tracker for **Munchkin Adventure Time** (Steve Jackson Games / USAopoly). Tracks 2–6 players and works out each one's combat strength against the monsters on the table.

**Combat strength** = Level + Gear + Allies + Character + Class + One‑shots − Curses

Per player:
- **Level** 1–10 (Level 10 wins)
- **Character** — the 8 character cards, with an On/Off switch for powers that only apply in some fights
- **Class** — Wizard / Royalty / Hero / Musician, with a **Super Munchkin** tick for a second class
- **Gear** — Headgear, Armor, Footgear, two hands (2‑handed tick), plus any number of Misc items, each with an On/Off switch for conditional cards
- **Allies**, **Curses**, and **One‑shots**

**The fight** — one or more monsters with level + modifier; every player card shows whether they beat the combined monster strength (ties go to the monster). **End battle** clears monsters and one‑shots; **New game** resets everything.

State is saved in the browser (`localStorage`), so the page can be closed mid-game and reopened on the same device.

## Run locally

It's a single static file — open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

## Deploy to Vercel

1. Push this repo to GitHub.
2. On Vercel: **Add New → Project → Import** the repo.
3. Framework preset **Other**; leave build command and output directory empty.
4. Deploy.

No environment variables, no build step, no backend.
