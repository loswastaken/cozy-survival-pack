# Cozy Survival pack

packwiz pack for Los's "Cozy Survival" server: Minecraft 1.20.1, Forge 47.4.28. Links only, no mod files.

Mods (server and client): Iron's Spells 'n Spellbooks, Botania, Ars Nouveau, YUNG's Better Dungeons, L_Ender's Cataclysm, Alex's Caves, Alex's Mobs, Naturalist, Critters and Companions, Just Enough Items, plus their libraries (Curios API, Patchouli, YUNG's API, Lionfish API, Citadel, GeckoLib, Architectury API, playerAnimator, Iron's Lib).
Client only: Embeddium (performance), Oculus (shaders), YetAnotherConfigLib.

Server: `dorkunify.duckdns.org:25569` (at home or on the VPN: `10.24.4.143:25569`). Whitelisted players only; send Los your Minecraft username first.

## Quick setup (one command)
Close Prism Launcher first.

Windows (PowerShell):

    irm https://raw.githubusercontent.com/loswastaken/cozy-survival-pack/main/join.ps1 | iex

macOS / Linux:

    curl -fsSL https://raw.githubusercontent.com/loswastaken/cozy-survival-pack/main/join.sh | bash

It installs Prism Launcher if needed, creates (or refreshes) the "Cozy Survival" instance, sets up the mod sync and adds the server. Then open Prism, sign in with your Microsoft account, and press Play. Read `join.ps1` / `join.sh` first if you like; they only touch Prism's own folder.

## Manual setup
1. Create a Prism instance named "Cozy Survival": Minecraft 1.20.1, Forge 47.4.28 (Java 17).
2. Download https://github.com/packwiz/packwiz-installer-bootstrap/releases/latest/download/packwiz-installer-bootstrap.jar into the instance's `.minecraft` folder.
3. Instance Settings > Custom commands > Pre-launch command:
   `"$INST_JAVA" -jar packwiz-installer-bootstrap.jar https://raw.githubusercontent.com/loswastaken/cozy-survival-pack/main/pack.toml`
4. Launch. Mods sync on every launch.
