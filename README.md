# FrameShift Command

**Current stable: v0.10.8** — a Windows desktop companion for Elite Dangerous: Odyssey.

[Download Windows x64 installer](https://github.com/Domo1702/frameshift-command-releases/releases/download/v0.10.8/FrameShift.Command_0.10.8_x64-setup.exe) · [Release notes and signatures](https://github.com/Domo1702/frameshift-command-releases/releases/tag/v0.10.8)

Existing updater-enabled installations can use **Settings → Check for updates → Update now**. Close FrameShift before running the manual installer. Microsoft WebView2 is required and can be downloaded by the installer. Node.js, Python and a separate server are not needed.

## Included

- Dashboard with Commander/Ship, Current System and Station panels, separate Mining/HGE/Exobiology discovery squares, live material-storage feedback and contextual search.
- Equal square material cards across Raw, Manufactured and Encoded, grades above artwork, separate Guardian/Thargoid rows, filters, watchlists, trade planning and engineer unlock guidance.
- Fleet/loadouts, stored modules, fitting and engineering drafts, saved-build comparison, import/export and bundled artwork.
- System/station search with a polished Outfitting console; consistent Missions panels and compact rows; HGE candidates with evidence and Copy; mining, cargo-aware market searches and route planning. Commodities includes All / Rare / Standard search with 142 rare goods. Provider reports do not guarantee stock or allocations.
- A compact Explorer overview with aligned Current System body/type/signal text and grouped Findings, routes, sampling, surface trackers and unsold estimates. Route discovery has visible Known / New / Unknown labels, with planet and arrival-star evidence explicitly distinguished. Multi-digit route numbers stay horizontal, and Copy retains the system-name action.
- Exobiology matching audited across 91 Odyssey species using 10,609 OD API calls and 9,908 unique synthetic comparisons. One shared condition table drives display predictions and notifications. Unique supported DSS matches show Species inferred; personal biological identification remains distinct. Limaxus and Radicoida automatic inference is withheld for documented API anomalies. Required composition, nebula distance, region, governing stars and material evidence must be known before automatic species naming. Missing inputs withhold inference; observed genera and actual discoveries remain visible. Electricae Radialem is withheld while nebula distance is unknown.
- Explorer route destination names use silver-grey for EDSM-known systems and soft copper-red for no returned community record, with subtle tints, labels and tooltips. Background checks use existing consent, six-hour caching, request pacing and replay isolation. Pending/error states remain neutral; journal discovery badges and Copy remain separate.
- Powerplay journal activity, pledged-power portraits, saved targets/notes and optional consented community intelligence.

The layout supports landscape and portrait windows, including 1080×960 half-screen use. v0.10.8 adds Explorer route community-coverage colours while retaining workspace polish, uniform material cards, rare commodity search and strict Exobiology matching. The build retains renderer recovery. The dashboard Exobiology square shows one current-system possibility notice and clears on jumping; detailed findings remain in Explorer. Popup windows are smaller, with existing delivery, position and duration settings preserved.

## Data and updates

Game journals are read-only. Existing Commander records, builds, layouts, settings and provider consent are retained during an update. External providers are opt-in. Predictions are estimates; they do not guarantee signals, organisms, drops or sale proceeds. Cartographic figures remain base estimates; Exobiology first-logged bonus totals are conditional.

The optional game overlay remains experimental; actual-game foreground/fullscreen and physical multi-monitor behavior still need user acceptance. App-only notifications are the default.

This repository distributes stable installers, detached signatures and the public update feed. Downloads require no GitHub account. The updater cryptographically verifies the original application signing key before installation. Windows Authenticode signing is not configured.

Before downgrading, retain a private backup of the production data directory shown in Diagnostics. Preview uses its own data directory; do not substitute a Preview database for production data.

Elite Dangerous and associated game assets belong to Frontier Developments. FrameShift Command is an independent companion application.

Discovery labels describe prior discovery when the scan was recorded. New does not guarantee a first-footfall bonus; Unknown is never presented as undiscovered. Copy continues to copy the destination system name.

Route colours describe EDSM coverage: no record does not prove nobody visited, and a known record does not establish full exploration. Enable Allow EDSM system lookups in Settings. Only destination system names are sent.
