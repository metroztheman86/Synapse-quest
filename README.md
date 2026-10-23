# Synapse (Quest)

Quest port of **Synapse** — a Beat Saber mod + server system for live synchronized events, in-game chat, shared leaderboards, and coordinated map starts.

This repository distributes the **compiled Quest package** (`.qmod`) for Beat Saber on Meta Quest.

> **Note:** This is a community/port build. The original PC mod and server are by [Aeroluna](https://github.com/Aeroluna).  
> Original PC repository: https://github.com/Aeroluna/Synapse

## Features (as described in the package)

- Reliable ~8-second stage handoff
- Parallel next-map preparation
- Bounded recovery
- Vivify-safe startup
- Countdown audio + custom event support
- Integration with the Synapse live-event directory

## Requirements

- Beat Saber **1.40.8_7379** (or the version listed in `mod.json`)
- Scotland2 modloader
- The dependencies declared in `mod.json` (automatically handled by most installers):

  | ID                    | Version   |
  |-----------------------|-----------|
  | beatsaber-hook        | ^6.4.2    |
  | custom-types          | ^0.18.3   |
  | bsml                  | ^0.4.55   |
  | songcore              | ^1.1.26   |
  | paper2_scotland2      | ^4.6.4    |
  | web-utils             | ^0.6.8    |

## Installation

1. Install a Quest mod manager (ModsBeforeFriday / QuestPatcher / BMBF, etc.).
2. Install the required core mods first if they are not already present.
3. Install `Synapse.qmod` from the [Releases](../../releases) page of this repository.
4. The countdown audio files are automatically copied to:
   ```
   /sdcard/ModData/com.beatgames.beatsaber/Mods/Synapse/Countdown/
   ```

## Configuration

By default the mod looks for an active event listing at:

```
https://synapse.totalbs.dev/api/v1/directory
```

You can change this by editing the config file on-device (exact path depends on the port; typically under the mod’s data folder).

## Credits

- **Original author:** [Aeroluna](https://github.com/Aeroluna) (PC mod + server)
- **Quest port:** Synapse Quest contributors
- License: MIT (see [LICENSE](LICENSE))
- Third-party notices: [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)

## Version

Current package: **1.2.22**

See `mod.json` for the exact package ID, game version, and dependency list.

## Disclaimer

Modding Beat Saber on Quest is unofficial and may violate Meta’s terms of service. Use at your own risk. This repository only redistributes the compiled package that was provided; it does not claim ownership of the original work.
