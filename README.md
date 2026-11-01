# FrameShift Command

**Current stable: v0.11.0** — a Windows desktop companion for Elite Dangerous: Odyssey.

[Download Windows x64 installer](https://github.com/Domo1702/frameshift-command-releases/releases/download/v0.11.0/FrameShift.Command_0.11.0_x64-setup.exe) · [Release notes and signatures](https://github.com/Domo1702/frameshift-command-releases/releases/tag/v0.11.0)

Existing updater-enabled installations can use **Settings → Check for updates → Update now**. Close FrameShift before running the manual installer. Microsoft WebView2 is required and can be downloaded by the installer. Node.js, Python and a separate server are not needed.

## New in v0.11.0

- **Fleet Carrier companion:** an owned-carrier overview with artwork, location, recorded tritium/capacity, services and jump history. A separate always-on-top desktop overlay shows the destination and saved scheduled-jump countdown. Position, text size, opacity, service row, lock, click-through and recovery controls are included.
- **Optional offline voice announcements:** Windows voices plus a searchable library of 28 Kokoro American/British English voices. Assign voices independently to HGE, Mining, Exobiology and Other, edit samples, select audio output and retain a Windows fallback. Announcements are off until enabled. The optional verified 148.4 MiB voice pack downloads only on request, runs locally on CPU and uses a bounded cache. No paid/cloud speech or Python is required; Piper, Qwen and GPU engines are not integrated.
- **Polished discovery notifications:** readable white headings and large outline icons, with green Exobiology, yellow Mining and orange HGE accents. Predicted/reported and identified/confirmed evidence use different shades. Exobiology scan cards show the body, supported species and evidence clearly; unknown species remain explicit.
- **Resizable discoveries:** stretch Current System Discoveries vertically, with saved height, keyboard resizing and reset. Mining, HGE and Exobiology retain their own scrollable panels and current-system scope.

## Included

- Commander/Ship, Current System and Station dashboard panels; contextual search and live material-storage feedback.
- Consistent material cards with grades, separate Guardian/Thargoid rows, filters, watchlists, trade planning and engineer progression/unlock guidance.
- Recorded fleet/loadouts, stored modules, fitting and engineering drafts, saved-build comparison, import/export and bundled artwork.
- System/station and Outfitting search, mission panels, HGE candidates with evidence and Copy, asteroid/planetary mining, cargo-aware commodity markets and trade planning. Commodities supports All / Rare / Standard searches with 142 rare goods; reported stock is not guaranteed.
- Compact Explorer overview, routes, grouped Exobiology findings, sampling, surface trackers, unsold Cartographic/Exobiology estimates and history. Known / New / Unknown route labels distinguish community coverage from personal scan evidence. Multi-digit route numbers and Copy remain readable.
- Audited Odyssey species conditions and optional separately consented Canonn reports. Missing required context withholds automatic species naming. Inferred species and personal identifications remain distinct.
- Powerplay journal pledge/rank/merits/activity, pledged-power portraits, targets/notes and optional consented community intelligence.

Responsive layouts support landscape and portrait windows, including 1080×960 half-screen use. Commander switching, Live/Legacy profiles, replay isolation, preferences and renderer recovery are retained.

## Data, overlays and updates

Journals remain read-only. Existing production Commander data, builds, layouts and provider consent are retained during updates. External providers are opt-in. Preview uses its own identity and data directory; its data is not copied into production.

The carrier countdown continues from its saved timestamp while FrameShift runs, even without new journal updates. Closing FrameShift removes the overlay; reopening restores the schedule. Expiry displays **Awaiting confirmation**, not a guaranteed completed jump. Cancellation, rescheduling, arrival and service changes require fresh recorded information. Services are last recorded, not remotely live. No game-control actions are added.

Predictions do not guarantee signals, organisms, drops or sale proceeds. Cartographic figures are base estimates; Exobiology first-logged bonus totals remain conditional. Community coverage does not prove a system has or has not been fully explored. Source age and unknown conditions remain visible.

Game overlays target windowed/borderless mode. Game-closed carrier display/countdown passed packaged checks. Actual-game exclusive fullscreen and physical overlay dragging/passthrough retain manual acceptance limits. App-only discovery notifications are the default. Carrier desktop-overlay visibility is independent of game focus.

This public repository contains stable installers, detached updater signatures and `latest.json`; application source remains private. Downloads require no GitHub account. The updater verifies artifacts against the original application signing key before installation. Windows Authenticode signing is not configured. No installer is executed automatically during release validation.

Before downgrading, export a private SQLite backup and preserve the production data and WebView preferences. Close FrameShift before changing versions. Never replace production data with a Preview database.

Elite Dangerous and associated game assets belong to Frontier Developments. FrameShift Command is an independent companion application; bundled AI artwork is illustrative.
