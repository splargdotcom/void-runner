# Changelog

## 1.3.2 — Deep Field

Maintenance follow-up to 1.3.1.

### Fixed

- Commit the Void Colossus sortie/cooldown lock only when `mkBoss()` succeeds, rather than when an ancient first answers the survey. A cancelled wind-up still consumes that ancient's stable examined result, but does not consume the global boss cooldown.
- Re-arm low/empty-fuel guidance when a new sortie begins.
- Remove the redundant `considerColossus()` call from `strikeRock()` and restore normal seam/off-seam extraction messaging.
- Calculate death score, death-screen kills/credits and leaderboard entry from the last docked checkpoint. Failed-sortie cargo and unbanked progress no longer inflate the wreck ledger.

### Unchanged by design

- No pirate waves were reintroduced.
- The Colossus remains a rare prospecting discovery, not a timed raid.
- 1.3 flight physics, camera behaviour, volumetric sectors, spatial dust/streaks and survey lattice are unchanged.
- Save compatibility remains on the existing checkpoint/career-event model.

## 1.3.1 — Deep Field

- Wired the Void Colossus into Red-sector ancient survey discovery using a stable per-body roll and diegetic telegraph.
- Removed disconnected timed pirate-wave content and `wave_clear` achievement/UI.
- Added in-memory restore to the last docked checkpoint on death.
- Added emergency-tow fuel guidance.
- Hid god mode behind `DEBUG = false`.
- Cleaned legacy state and improved new-run reset and pause/gamepad handling.

## 1.3 — Space & Flight

- Rebuilt asteroid placement into sector-specific 3D formations.
- Added torque-based rotational flight and meaningful assist-off coasting.
- Added spring-arm chase camera, dynamic FOV, subtle banking and responsive engine flare.
- Added near/mid spatial particles, speed streaks and a local 3D survey lattice.
- Added three-axis asteroid tumble.
