# Nexus Relay — source-code consolidation plan

**Central product page:** [Nexus Relay](../README.md)

This is a **non-destructive repository consolidation plan**, not proof that all three programs already run from one build.

## Current source repositories
- `Cardsmageanime/Arcade-Nexus`: virtual arcade, Godot-oriented 2D world and museum (proposed main home).
- `Cardsmageanime/RetroRelay`: Python desktop/lobby server; early source-code preview.
- `Cardsmageanime/RetroVerse` branch `milestone/arm64-kernel-build-20261023`: ARM64 kernel/initramfs and read-only SD/boot tools.

## Future unified source layout (target, not yet created)
```text
nexus-relay/
  apps/
    arcade-world/              # 2D/3D world client
    desktop-relay/             # RetroRelay desktop app
    arm-systems/               # ARM Linux build and hardware profiles
  services/
    relay-lobbies/             # Online identity, match/lobby APIs
    partner-store/             # Rights-gated marketplace (not operational)
  packages/
    contracts/                 # APIs and event schemas across components
    design-system/             # original UI assets only
  docs/
    museum/
    learning/
    hardware/
```

## Integration order
1. Inventory tracked files, binary art, licenses, secrets, runtimes, test commands and build artifacts in all repos; quarantine any unverified asset.
2. Establish contract schemas for library items, profiles, game identity, multiplayer session compatibility and offline state.
3. Import version-controlled code preserving traceability to original commits, keeping independent build/test commands; avoid blindly copying virtual environments, firmware, ROMs, credentials or binary releases.
4. Stand up cross-component smoke tests and shared UI navigation. Maintain the ARM safety gates (no Android/eMMC writes or boot with unverified DTB).
5. When tests pass, consider a repository-name migration and update GitHub links and scheduled biweekly automation. Do not remove source repos until owner review.
6. Publisher Store remains conceptual until rights, seller verification, payments, refunds, taxes, security and licensing are properly implemented.

## Current result
The GitHub **landing pages** have been consolidated under the Nexus Relay identity and link to the existing codebases. The **actual Git histories and executable source trees remain separate** pending a safe implementation migration. Phases 1–5 are authorized; Phase 6 is explicitly off-limits.
