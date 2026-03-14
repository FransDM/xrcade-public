# XRcade Manager

Admin application for location-based entertainment (LBE) VR venues. Use it to monitor and control VR headsets, run and manage Spatial Ops matches, and display live game overlays.

**Author:** XRcade Belgium

Current version: v1.0.2

---

## What It Does

- **Headsets** — View all configured headsets (connection, battery, WiFi, ADB). Start/stop streaming (scrcpy or RTMP), enable stay-on, pause guardian, and run other device actions.
- **Spatial Ops Manager** — Control the Spatial Ops game via the XRcadeSOMod (MelonLoader): players, squads, match rulesets, bot count, and game commands (start, stop, etc.).
- **Monitor** — Live match view with multiple themes (Futuristic, Retro, Office, Dark/Light Colorful): scoreboard, lobby, and real-time events over SSE.
- **Matchmaker** — Plan sessions: create teams, assign players and headsets, generate round-robin schedules.
- **Overlays** — OBS-ready overlay pages (e.g. futuristic team/player layouts) for streaming.
- **Settings** — Session, match, and mod options; license activation (HWID-bound).

The app talks to the game through the mod’s HTTP API and can be packaged as a Windows executable for venue PCs.

---

Open [http://localhost:9520](http://localhost:9520).

Version 1.0.1-beta release-notes
- added support for multiple monitors
- added monitor modes: Schedule / Game / Scoreboard
  * Schedule: Shows scheduled matches (views: Next-up, Loop)
  * Game: Shows game information (views: Lobby, Match, Result)
  * Scoreboard: Shows the past scores (views: Last, Loop)
- added OBS management to Monitor & streaming section
- implemented OBS orchestrator (changes scenes automatically, loops player streams or monitor streams, auto-reverts to default scene - can be taylored to your needs)
- headset management updates
  * added launch Spatial ops on all headsets button
  * added relaunch Spatial Ops on all headsets button
  * implemented relaunch Spatial Ops per headset functionality (right-click button)
  * added controller battery level information and warning toggle on set battery level
  * added volume controle and auto-volume reset option
  * [experimental] added a button to clear Meta spatial data
  * [experimental] added a button to clear guardian data
  * [experimental] added a button to clear mrds data
    [important] Use experimental features at your own risk (!) this has been tested and works, but removes files using ADB and isn't without risk.
- added Sessions
  * schedule matches with predefined settings, players, bots, maps
  * have matches be auto-prepared so you just have to hit Start match to get started
- streaming optimizations
  * OBS-profile fixes and performance improvements (moved from webm to mkv H.264 for background videos, made scripts & shaders a lot more effective, removed "reconnecting" backgrounds)
  * added 3 monitor views to OBS
  * added 3 custom scenes to OBS
  * added 1plus3 viewing mode (auto-switched) for Blue/Orange&player streaming (showing top players and auto-switching the streams)
  * OBS assets overlay UI improvements
- Updated player view while not in match
- updated the Settings-page so everything is easier to find
- tons of UI updates and label changes for better overall User Experience
