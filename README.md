# FrameShift Command

A Windows desktop companion for **Elite Dangerous: Odyssey**. Follow your Commander, ships, engineering materials, markets, exploration and Powerplay activity through live, read-only journal updates.

**Current stable build: v0.10.0**

[Download the Windows x64 installer](https://github.com/Domo1702/frameshift-command-releases/releases/download/v0.10.0/FrameShift.Command_0.10.0_x64-setup.exe) · [Release notes and assets](https://github.com/Domo1702/frameshift-command-releases/releases/tag/v0.10.0) · [Latest stable release](https://github.com/Domo1702/frameshift-command-releases/releases/latest)

## New in v0.10.0

- **Explorer & Exobiology:** journal-driven system and body analysis, route import/export, sampling progress, surface trackers and discovery-value estimates.
- **Exobiology Intelligence:** Known/Predicted/Confirmed evidence, body analysis and recommended in-app targets, using 21 documented environmental species conditions.
- **Optional Canonn reports:** consented system lookups, cached community sightings and offline fallback. Community reports remain distinct from your own confirmed discoveries.
- **Discovery notices:** configurable three-second alerts inside FrameShift or at the top/bottom of a borderless/windowed game screen.
- **Powerplay:** personal pledge, rank, merits and journal activity, locally observed systems, saved targets, notes and strategy tools.
- **Material collection notices:** live dashboard feedback showing how much storage remains for each material collected.

These features are combined in the stable application, alongside the existing dashboard, fleet, engineering, mining and market tools.

## Main features

| Area | What you can do |
| --- | --- |
| Command dashboard | See journal-derived Commander/ship statistics, current-system details, station services and contextual arrival notices. |
| Materials & Engineering | Browse Raw, Manufactured and Encoded stock, filter by grade/search, plan trades, watch shortages, follow engineer progression and unlock requirements, and navigate surface targets. |
| Ships & Builds | Review your fleet, recorded loadouts and stored modules; plan and compare builds; import/export FrameShift JSON and SLEF. Includes Anaconda Mk II support and bundled ship artwork. |
| Galaxy intelligence | Search systems/stations/services, find evidence-labelled HGE candidates and copy destination system names. |
| Mining & Commodities | Explore reported hotspots and prospecting candidates, planetary resource searches, cargo-aware Buy/Sell searches, routes and market alerts. |
| Explorer & Powerplay | Track routes, bodies, biological sampling, journal discoveries and personal Powerplay activity in the same application. |
| Profiles & layout | Switch Commanders, retain separate Live/Legacy profiles, use isolated simulated replay, and resize for landscape or portrait windows, including a 1080 × 960 half-screen arrangement. |

## Install and connect

1. Download **FrameShift.Command_0.10.0_x64-setup.exe** from this repository's release assets.
2. Close FrameShift Command and run the installer.
3. Launch **FrameShift Command**, then connect the detected journal folder or choose **Settings → Browse → Import & watch**.
4. The usual folder is `%USERPROFILE%\Saved Games\Frontier Developments\Elite Dangerous`.
5. Select your Commander and enable any wanted external providers individually in Settings.

The application runs locally on Windows x64. Node.js, Python and a separate server are not needed. Microsoft WebView2 is required; the installer can download it if absent. Game journal files remain read-only. No API key is needed for local tracking and planning.

## Automatic updates

Existing updater-enabled installations can use **Settings → Check for updates**. The stable app checks on startup and every six hours when automatic checks are enabled. A newer release shows its notes; installation starts when you select **Update now**.

Installer updates are cryptographically signed and verified by the app. The installer has no Windows Authenticode signature, so Windows may show a publisher warning. No GitHub login is required to download or update.

Builds through v0.1.24 need a manual installation of a newer updater-enabled build first.

## Privacy and data

- Commander records, inventory and imported journals are stored locally.
- EDSM, Spansh, Canonn and on-demand AI features require their respective consent.
- Canonn biology lookups are off by default and send only the current system name/address, not your Commander name or journals.
- AI Search is optional, requires your API key and separate sharing consent, and can incur provider charges. Windows Credential Manager stores the key.
- Software-update requests do not upload Commander records or journals.
- Production and the combined Preview app have separate data directories. Preview notes/preferences are not automatically copied into stable v0.10.0.
- Use **Export SQLite backup** before replacing data or downgrading. Close the app before restoration and retain the original data until recovery is verified.

## Evidence and current limitations

HGE candidates are predictions, not guaranteed signals or material drops. Mining and market reports depend on provider coverage and source age.

Exobiology estimates separate base values from a conditional first-logged bonus scenario. First footfall and bonus eligibility remain unverified; recorded journal sales are confirmed earnings. Unsupported species/variant rules and missing environmental inputs remain unknown.

Powerplay tracks personal/local observations. An authorised galaxy-wide Powerplay 2 index and full cascade forecasts are unavailable.

Automated Windows tests cover notification lifecycle and placement. Automatic discovery triggering with Elite Dangerous actually in the foreground still requires live-game acceptance. Paid AI execution remains unverified.

## Release verification

v0.10.0 passed TypeScript validation, **421 frontend tests, 79 Rust tests and 115 browser tests**, plus packaged Windows checks. An isolated upgrade from the real v0.9.1 executable preserved balances, inventory, ships, preferences and journal offsets. The older app detected and signature-verified the official v0.10.0 update; v0.10.0 correctly reports itself up to date.

Installer SHA-256:

```text
DC8C200C977A2B07D707024B3BC91AF8B2A464D90698F95E876A484FB90FEAC1
```

## About this repository

This is the **public stable distribution repository**. Releases contain the Windows installer, its detached updater signature and `latest.json`. Application source stays private; no journals, databases, API keys or signing secrets are distributed here. Stable private source uses `master`; shared development/testing uses one `preview` branch.

Elite Dangerous and associated game assets belong to Frontier Developments. FrameShift Command is an independent companion app. Bundled artwork is illustrative.
