# AlvOps

Self-hosted first. I build homelab plumbing, game tooling, and AI agent infrastructure.

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

Everything else lives in the repository list below.
