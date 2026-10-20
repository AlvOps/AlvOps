# AlvOps

Self-hosted first. I build homelab plumbing, game tooling, and AI agent infrastructure.

## Darmstadt Public Transport Map

**[darmstadt-live-map](https://github.com/AlvOps/darmstadt-live-map)** — a live-only map of Darmstadt's trams, buses and S-Bahn/regional trains, served at **[darmstadtmap.com](https://darmstadtmap.com/)**.

- **Live, never scheduled** — the timetable replay it grew out of was deleted; markers come from realtime feeds or the operator's own GPS, and a GPS position is drawn differently from one derived from stop prognoses
- **Answers "where is *my* bus?"** — picking a line strips the map to that line alone (stops come back after 10 s of quiet), picking a vehicle leaves only that vehicle, its route and its next stops
- **Operator and open feed in one view** — HEAG's own positions where they exist, DELFI/MOTIS prognoses for everything else, with per-vehicle provenance in the popup
- **Bilingual by default** (EN/DE), phone-first layout, and RMV service notices in a bottom bar that says plainly when the notice feed is down

## ffx-wayland-lightning-dodger-x2speed

**[ffx-wayland-lightning-dodger-x2speed](https://github.com/AlvOps/ffx-wayland-lightning-dodger-x2speed)** — a performance-oriented auto lightning dodger for *Final Fantasy X HD Remaster* running natively on Linux through Steam/Proton.

- **Wayland native** — samples raw pixel data straight from the compositor with `grim`, no X11
- **Kernel-level input** — injects keystrokes through `evdev` / `/dev/input/uinput`, bypassing the SDL2/Proton hooks that ignore userspace-simulated keys
- **x2 game speed** — a sustained background key-hold thread keeps the engine's input buffer fed even at double speed
- One-command installer (`setup.sh`) for packages, udev rules and permissions

## wow-mcp-forever

**[wow-mcp-forever](https://github.com/AlvOps/wow-mcp-forever)** — an MCP server that answers
*World of Warcraft: Forever* questions directly from the Wowhead database: where an item drops, who
sells it, which quest starts a chain, full tooltip stats, drop chances and reward tables.

- One call per question — `forever_find` searches by name and returns the best match with full details
- Every answer carries a `source` URL so it can be cited
- Drop-in for any MCP client, no API keys, MIT licensed

## hermes-credits-plugin

**[hermes-credits-plugin](https://github.com/AlvOps/hermes-credits-plugin)** — an OpenRouter credits chip and pane for the Hermes desktop app: live balance, quota and budget bars, and a per-conversation call log so you can see what each chat actually costs.

## twitch-folders

**[twitch-folders](https://github.com/AlvOps/twitch-folders)** — a browser extension that sorts the Twitch channels you follow into your own folders, so the sidebar stops being one endless list.
Featured in : https://addons.mozilla.org/en-US/firefox/addon/twitch-folders/

Everything else lives in the repository list below.
