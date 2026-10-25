# Arcade Nexus

**Your Games. Your Universe. One Launcher.**

Arcade Nexus is a planned free, open-source **2D side-scrolling virtual arcade launcher** for Linux Mint first and Windows later. Walk through an arcade world, interact with cabinets representing local PC games and compatible emulators, and launch games you already own. An optional **3D virtual arcade upgrade is planned for 2028**, while retaining the 2D experience.

**Join the project, suggest features through GitHub Issues, and help build the ultimate gaming hub!**

## Development roadmap (2026–2028)

**Planning baseline:** October 25, 2026 (America/Chicago). All dates are targets, not guaranteed releases. Only verified commits and tests count as completed work.

| Target | Milestone | Planned deliverable | Status |
| --- | --- | --- | --- |
| Oct–Nov 2026 | v0.1 2D foundation | Godot 4 project, side-scrolling room, avatar movement and camera | Planned |
| Nov–Dec 2026 | v0.1 cabinet interaction | Interactive cabinets, local library and safe game launching | Planned |
| Dec 2026–Jan 2027 | v0.2 2D expansion | Emulator configuration, game collections, artwork and favorites | Planned |
| Q1–Q2 2027 | v0.3 2D world and museum prototype | Multiple themed rooms, controller navigation, NES-first exhibits and localization framework | Planned |
| Q3 2027 | My Games Lobby and multilingual museum expansion | Library discovery, Windows testing, chronological console halls, sourced sales displays and translated exhibits | Planned |
| Q4 2027 | Online lobby, arcade netplay adapters and library sync prototype | Account security, public/private rooms, compatible online game launch, invitations and opt-in catalog sync | Planned |
| Q1 2028 | 3D prototype and personal avatars | Third-person movement, walkable 3D arcade room and basic customizable avatar | Planned |
| Q2 2028 | 3D interaction and avatar customization | Interactive 3D cabinets, controller support, avatar clothing, hairstyles and accessories | Planned |
| Q3 2028 | Shared social world and personal arcade homes | Game library, museum, online lobbies, visible multiplayer avatars and personal home prototype | Planned |
| Q4 2028 | 3D world and home release candidate | Personal home customization, visitor privacy, performance, accessibility, security and packaging tests | Planned |

**Release policy:** 2D remains available when 3D is introduced. The 3D release proceeds only after validation. These milestones supersede the earlier Python/PySide6 desktop-only schedule and January 2027 v1.0 assumption.

## 2028 3D Virtual Arcade World and Avatars (planned)

- Each player can create and customize a personal 3D avatar (appearance, hairstyles, clothing, colors and accessories), with settings saved locally and optionally synced to an authenticated account.
- Explore walkable 3D arcade halls, a gaming history museum, and a personal My Games Lobby; interact with cabinets to launch owned games or compatible online sessions.
- Support public and private shared social spaces with visible player avatars, friends and invitations; implement authoritative networking, privacy settings, moderation and scalable player limits before release.
- Reuse the 2D launcher backend, museum records, translations and account/lobby services. **Keep 2D mode playable** rather than replacing it.
- Stage the 2028 delivery: Q1 movement/avatar prototype; Q2 customization and cabinet interactions; Q3 shared social world integration; Q4 performance, security and release-candidate testing.

**Status:** Design requirement only; no 3D world, avatar creator or shared-world networking implemented or tested.

## Personal Arcade Homes (planned for 2028)

- Every player can create a customizable personal arcade home, beginning with a starter room and optional expansion.
- Place and rearrange furniture, lighting, wall/floor themes, arcade cabinets and game-collection displays; support saving and restoring layouts.
- Show a player's chosen games and collections as metadata/artwork displays, subject to privacy settings and asset permissions. Visitors cannot access the owner's local game files or platform credentials.
- Invite friends for social visits, shared hangouts and compatible online matches. Actual multiplayer gameplay remains dependent on supported game/emulator integrations.
- **Friends-only by default**: only mutually approved friends may visit. Owners can change to private (only owner), invite-only, or public discovery. Provide access revocation, block/report tools, owner moderation, and a clear privacy choice during onboarding. Never automatically expose a new home to strangers.
- Store home layouts locally and support opt-in authenticated sync; protect account data and validate user-created content.
- Target Q3 2028 for a basic home prototype and Q4 2028 for customization, privacy and multiplayer visitor testing. These are estimates, not release commitments.

**Status:** Planned only; no home builder, persistence or multiplayer visiting has been implemented.

## Gaming History Museum (planned)

- A walkable, side-scrolling museum starting with the **NES/Famicom era**, progressing chronologically through console generations to modern gaming; preserve accurate regional launch dates.
- Each console exhibit: manufacturers and developers, hardware specifications, development history, announcements, regional debuts, major milestones and cultural impact.
- Each featured game: release date by region, credited creators/studios, development history, debut, platform versions and legacy.
- Show **top 10 best-selling games per console** when credible comparable data exists; cite sources, define worldwide versus regional sales, distinguish shipped versus sold-through figures and label estimates/unknowns. Never fabricate a complete top ten.
- Museum data must be maintained as structured, sourced records; accessible exhibit panels, search and chronological timeline.
- Historical exhibits are viewable without owning games. Optional **Play** actions only appear for locally installed, legally accessible games with compatible launch configuration.
- Begin with an NES hall and a small set of verified exhibits, then expand to Sega, Nintendo, Sony, Microsoft, handhelds, PC and other systems; future 3D mode should reuse the same exhibit database.
- Do not imply manufacturer endorsement; use only assets with appropriate rights.

**Status:** Museum concept and requirements recorded; exhibit database and game scenes are not yet implemented.

## Multilingual support (planned)

- **Scope:** Localize the full Arcade Nexus experience, not just the museum: menus, settings, My Games Lobby, online lobby controls, errors, accessibility text and historical exhibit content.
- **Initial target languages:** English (source), Spanish, French, German, Portuguese (Brazil), Japanese, Simplified Chinese and Korean. Additional languages can follow with community translation support.
- **Language selection:** First-run language picker, manual change in settings, and optional system-language detection with English fallback. A language change should not require an online account.
- **Implementation:** Godot 4 translation resources/CSV or PO catalogs with stable translation keys; separate historical exhibit content from interface strings. Support Unicode fonts, text expansion, localized dates and numbers, and language-specific search where practical.
- **Quality:** Review translations for accuracy, especially console names, release regions, sales terminology and historical claims. Mark missing translations and fall back gracefully; do not present machine translations as reviewed.
- **Future readiness:** Plan right-to-left layout and font testing before adding Arabic or other RTL locales. Both 2D and 2028 3D modes should use the same translation resources.

**Status:** Language requirements documented only; translation assets and translated interfaces are not implemented yet.

## My Games Lobby and reserved libraries (planned)

- Dedicated in-world **My Games Lobby** to browse, search, favorite and launch games from the player's collections.
- Import or discover local installations and library metadata from supported Steam, Epic Games, GOG and configured emulator folders, using supported integrations and user permission.
- Save the user's **library catalog metadata** to their Arcade Nexus account only with explicit opt-in, enabling restoration/sync across devices; keep a usable offline local catalog.
- Sync does **not** upload commercial game binaries, copyrighted ROMs, third-party credentials, license entitlements or save files by default. Game installations and platform ownership checks remain subject to their original services.
- Include privacy controls, export/delete options, conflict resolution and secure authenticated sync; local paths are device-specific and must be remapped on another computer.
- Reserve room for future cloud-save integrations only when supported and authorized; not part of the initial sync promise.

**Status:** Requirements recorded; no import adapters, cloud storage or account sync implemented or tested.

## Planned online multiplayer lobbies

- Public, private and friends-only rooms, invitations, presence and room codes.
- Optional social arcade hub with visible player avatars; spectator rooms only where game/emulator streaming or spectating is supported.
- Host moderation: room locks, kick/mute/report/block controls.
- Cross-platform lobby discovery for Linux/Windows when supported; actual netplay compatibility depends on the game/emulator and matching versions.
- Security: authenticated online accounts, secure sessions, rate limiting, abuse reporting, and privacy controls. Never expose player IP addresses in the UI.
- Offline single-player remains fully functional without a login.
- A lobby is not an emulator or netcode engine: launching a game together does not itself provide multiplayer to unsupported titles.

**Status:** Concept approved for planning only. No lobby server, authentication or netplay integration has been implemented or tested.

## Online arcade gameplay (planned)

- Interactive arcade cabinets may offer Single Player, Online Versus, Public Match, Private Match, Spectate, Rematch and Game History **only when the selected game and integration actually support each action**.
- Example use case: Marvel vs. Capcom fighting games. The particular arcade version, emulator/core, networking method, rights and game ownership requirements must be checked before enabling online play.
- Use existing authorized game networking or compatible emulator netplay integrations (potentially Fightcade/FBNeo or RetroArch where supported); Arcade Nexus does not create universal netcode or grant game licenses.
- Matchmaking/lobby coordination is separate from actual game networking. Check game/core versions, ROM compatibility where applicable, controller mapping and connection requirements before a match.
- Preserve local/offline play. Apply account security, moderation and privacy controls to online rooms. Never advertise a mode as supported until it passes real multiplayer testing.
- Reuse the same game-specific online capability metadata and lobby backend in the future 3D arcade.

**Status:** Planned only; no netplay adapters or online matches implemented or verified.

## Development reviews

**Requested cadence:** Monthly, first Sunday of each month, America/Chicago. Automatic scheduling is **not active** because the scheduled-task limit was reached. At each review, record the actual date/time, verified commits and tests, work in progress, blockers, next steps, and revised estimates. If no development occurred, report that plainly.

### Update log

| Date (America/Chicago) | Verified update |
| --- | --- |
| 2026-10-25 | Roadmap revised for Godot-based 2D side-scrolling virtual arcade and planned 2028 3D upgrade; implementation remains planned. Online multiplayer lobbies and My Games Lobby with local library imports and optional catalog sync added to the planned roadmap; no online services implemented. |

## Technology and principles

- Godot 4 with GDScript for the 2D world and future 3D scenes
- Shared local game library and safe launcher backend for both modes
- Offline-first, keyboard and controller navigation
- Linux Mint first; Windows later
- Arcade zones can organize games by system without implying official console manufacturer partnerships
- No bundled copyrighted ROMs, proprietary firmware, or newly implemented emulators

## Detailed design

See [Side-Scrolling Arcade Plan](docs/SIDE_SCROLLING_ARCADE_PLAN.md), including the 2028 3D World Upgrade.

## Contributing

Open a GitHub Issue with a feature idea or bug report. Contributions and testing feedback are welcome.
