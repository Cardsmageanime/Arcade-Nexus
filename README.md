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
| Q1–Q2 2027 | v0.3 2D world | Multiple themed arcade rooms, controller navigation, customization | Planned |
| Q3 2027 | v0.4 platform support | PC store integration research, Windows support and stability testing | Planned |
| Q4 2027 | Online lobby prototype | Account security, public/private rooms, invitations and basic presence | Planned |
| Q1 2028 | 3D prototype | Third-person avatar and walkable 3D arcade room | Planned |
| Q2 2028 | 3D interaction | Interactive 3D cabinets, navigation and controller support | Planned |
| Q3 2028 | Shared 2D/3D library and lobbies | Game library, launch functionality, settings and compatible online lobby access in both modes | Planned |
| Q4 2028 | 3D release candidate | Performance, accessibility, packaging and hardware testing | Planned |

**Release policy:** 2D remains available when 3D is introduced. The 3D release proceeds only after validation. These milestones supersede the earlier Python/PySide6 desktop-only schedule and January 2027 v1.0 assumption.

## Planned online multiplayer lobbies

- Public, private and friends-only rooms, invitations, presence and room codes.
- Optional social arcade hub with visible player avatars; spectator rooms only where game/emulator streaming or spectating is supported.
- Host moderation: room locks, kick/mute/report/block controls.
- Cross-platform lobby discovery for Linux/Windows when supported; actual netplay compatibility depends on the game/emulator and matching versions.
- Security: authenticated online accounts, secure sessions, rate limiting, abuse reporting, and privacy controls. Never expose player IP addresses in the UI.
- Offline single-player remains fully functional without a login.
- A lobby is not an emulator or netcode engine: launching a game together does not itself provide multiplayer to unsupported titles.

**Status:** Concept approved for planning only. No lobby server, authentication or netplay integration has been implemented or tested.

## Development reviews

**Requested cadence:** Monthly, first Sunday of each month, America/Chicago. Automatic scheduling is **not active** because the scheduled-task limit was reached. At each review, record the actual date/time, verified commits and tests, work in progress, blockers, next steps, and revised estimates. If no development occurred, report that plainly.

### Update log

| Date (America/Chicago) | Verified update |
| --- | --- |
| 2026-10-25 | Roadmap revised for Godot-based 2D side-scrolling virtual arcade and planned 2028 3D upgrade; implementation remains planned. Online multiplayer lobby features added to the planned roadmap; no online services implemented. |

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
