# FrameShift Command

**Current stable: v0.10.5** — a Windows desktop companion for Elite Dangerous: Odyssey.

[Download Windows x64 installer](https://github.com/Domo1702/frameshift-command-releases/releases/download/v0.10.5/FrameShift.Command_0.10.5_x64-setup.exe) · [Release notes and signatures](https://github.com/Domo1702/frameshift-command-releases/releases/tag/v0.10.5)

Existing updater-enabled installations can use **Settings → Check for updates → Update now**. Close FrameShift before running the manual installer. Microsoft WebView2 is required and can be downloaded by the installer. Node.js, Python and a separate server are not needed.

## Included

- Dashboard with Commander/Ship, Current System and Station panels, separate Mining/HGE/Exobiology discovery squares, live material-storage feedback and contextual search.
- Materials inventories, grade filters, watchlists, engineering shortages, trade planning, engineer progression and unlock guidance.
- Fleet/loadouts, stored modules, fitting and engineering drafts, saved-build comparison, import/export and bundled artwork.
- System/station search, HGE candidates with evidence and copy controls, mining locations, commodities, cargo-aware market searches and route planning.
- A compact Explorer overview with grouped Findings, routes, sampling, surface trackers and unsold estimates. Prior-discovery markers distinguish previously discovered, undiscovered when scanned and unknown bodies. System route stops now show the same icons for the recorded arrival star, and multi-digit route numbers stay horizontal.
- Exobiology matching audited across 91 Odyssey species using 10,609 OD API calls and 9,908 unique synthetic comparisons. One shared condition table drives display predictions and notifications. Unique supported DSS matches show Species inferred; personal biological identification remains distinct. Limaxus and Radicoida automatic inference is withheld for documented API anomalies. Missing data stays explicit, and actual discoveries remain visible.
- Powerplay journal activity, pledged-power portraits, saved targets/notes and optional consented community intelligence.

The layout supports landscape and portrait windows, including 1080×960 half-screen use. v0.10.5 includes the HMC Caputus correction and broader audited body/atmosphere, temperature, pressure, gravity, composition, region and star conditions. The build retains renderer recovery. The dashboard Exobiology square shows one current-system possibility notice and clears on jumping; detailed findings remain in Explorer. Popup windows are smaller, with existing delivery, position and duration settings preserved.

## Data and updates

Game journals are read-only. Existing Commander records, builds, layouts, settings and provider consent are retained during an update. External providers are opt-in. Predictions are estimates; they do not guarantee signals, organisms, drops or sale proceeds. Cartographic figures remain base estimates; Exobiology first-logged bonus totals are conditional.

The optional game overlay remains experimental; actual-game foreground/fullscreen and physical multi-monitor behavior still need user acceptance. App-only notifications are the default.

This repository distributes stable installers, detached signatures and the public update feed. Downloads require no GitHub account. The updater cryptographically verifies the original application signing key before installation. Windows Authenticode signing is not configured.

Before downgrading, retain a private backup of the production data directory shown in Diagnostics. Preview uses its own data directory; do not substitute a Preview database for production data.

Elite Dangerous and associated game assets belong to Frontier Developments. FrameShift Command is an independent companion application.
