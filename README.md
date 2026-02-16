# XRcade Manager

Admin application for location-based entertainment (LBE) VR venues. Use it to monitor and control VR headsets, run and manage Spatial Ops matches, and display live game overlays.

**Author:** XRcade Belgium

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
