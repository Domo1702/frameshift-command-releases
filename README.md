# FrameShift Command

**Current stable: v0.12.2** — a Windows desktop companion for Elite Dangerous: Odyssey.

[Download Windows x64 installer](https://github.com/Domo1702/frameshift-command-releases/releases/download/v0.12.2/FrameShift.Command_0.12.2_x64-setup.exe) · [Release notes and signatures](https://github.com/Domo1702/frameshift-command-releases/releases/tag/v0.12.2)

Existing updater-enabled installations can use **Settings → Check for updates → Update now**. Close FrameShift before running the manual installer. Microsoft WebView2 is required and can be downloaded by the installer. Node.js, Python and a separate server are not needed.

## New in v0.12.2

- Compact 88-pixel material cards across Raw, Manufactured, Encoded, Guardian and Thargoid rows. Grade above the icon, material name and owned/maximum count stay visible; card progress bars are removed. Existing tabs, filters, family headings, favorites and details are retained.
- Correct material bundle overflow: when 199 of 200 slots are occupied, a three-unit pickup accepts one. Later crafting, trades and rewards use the corrected inventory.
- One-time retained-journal inventory repair corrects saved over-counts and subsequent consumption. Full journal snapshots remain authoritative; unverified special-material limits remain unknown. Other Commander state, layouts, consent and journal offsets are preserved.

## Included

- Fleet Carrier overview/services/history and its independent desktop jump overlay; optional offline Windows voices and 28 Kokoro English voices with saved category assignments.
- Commander/Ship, Current System and Station dashboard panels; contextual search and live material-storage feedback.
- Compact material cards with grades and clear owned/maximum counts, separate Guardian/Thargoid rows, filters, watchlists, trade planning and engineer progression/unlock guidance.
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

The combined release is verified with frontend/backend tests, responsive browser checks, packaged synthetic journal acceptance, production upgrade checks and original-key signed updater verification. Actual gameplay, physical monitor/DPI and audible audio acceptance remain manual.

This public repository contains stable installers, detached updater signatures and `latest.json`; application source remains private. Downloads require no GitHub account. The updater verifies artifacts against the original application signing key before installation. Windows Authenticode signing is not configured. No installer is executed automatically during release validation.

Before downgrading, export a private SQLite backup and preserve the production data and WebView preferences. Close FrameShift before changing versions. Never replace production data with a Preview database.

Elite Dangerous and associated game assets belong to Frontier Developments. FrameShift Command is an independent companion application; bundled AI artwork is illustrative.
