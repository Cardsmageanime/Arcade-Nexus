# Arcade Nexus — Side-Scrolling Virtual Arcade

## Confirmed direction (October 25, 2026)
Arcade Nexus is an offline-first, side-scrolling 2D virtual arcade launcher for Linux Mint initially, with Windows support planned. Players walk left and right through arcade rooms, interact with cabinets, browse their own local game collections, and launch installed games or compatible emulators. No bundled copyrighted ROMs or proprietary console software.

## Architecture
- **Engine:** Godot 4 (GDScript) for 2D rendering, input, camera, UI, and room transitions.
- **Library:** locally saved game metadata and configured launch commands; validate paths before execution.
- **Launching:** explicit, user-configured executables and arguments; avoid arbitrary shell execution.
- **Platforms:** themed collections are organizational labels, not claims of official support or partnerships.
- **Initial target:** Linux Mint desktop; Windows port after testing.

## v0.1 acceptance criteria
1. A runnable Godot project opens to one horizontal arcade room.
2. A player avatar moves left/right with keyboard and can stop near a cabinet.
3. Interaction opens a cabinet-specific menu; cancel returns to the room.
4. Users can register at least one installed game with executable path and arguments.
5. Selecting a registered game launches it with error handling.
6. Local settings persist across restarts and all core features work offline.
7. Source, setup steps, and manual test checklist are documented.

## Proposed implementation sequence
1. Project scaffold, room scene, player movement, camera.
2. Cabinet interaction area and library menu.
3. Local library persistence and safe launch adapter.
4. Keyboard/controller navigation, packaging, and smoke tests.

## Later milestones
- Multiple rooms and platform-themed zones (arcade, Nintendo, Sega, PlayStation, Xbox, handhelds, PC).
- Artwork, soundtracks, favorites, search, customizable avatar and arcade decorations.
- Supported emulator discovery, controller refinements, Windows compatibility.

## Roadmap and review policy
The previous Python/PySide6 desktop-only timeline is superseded by this Godot-based 2D direction. Estimated first prototype: 2–4 weeks of active development; fuller initial release: approximately 3–5 months, subject to testing. Review monthly, recording actual timestamp (America/Chicago), verified commits/tests, blockers, and revised milestones. Scheduling an automatic monthly review requires a free task slot.

**Status:** Specification recorded; prototype code and testing not yet completed.
