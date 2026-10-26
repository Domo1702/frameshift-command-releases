# FrameShift Command

A Windows desktop companion for **Elite Dangerous: Odyssey**. Follow your Commander, ships, engineering materials, markets, exploration and Powerplay activity through live, read-only journal updates.

**Current stable build: v0.10.1**

[Download the Windows x64 installer](https://github.com/Domo1702/frameshift-command-releases/releases/download/v0.10.1/FrameShift.Command_0.10.1_x64-setup.exe) · [Release notes and assets](https://github.com/Domo1702/frameshift-command-releases/releases/tag/v0.10.1) · [Latest stable release](https://github.com/Domo1702/frameshift-command-releases/releases/latest)

## New in v0.10.1

- **Current-system discoveries:** detailed coloured dashboard cards show all retained findings from your current visit in a compact scrollable area. Jumping hides previous visits; returning does not restore older notices.
- **Grouped mining notices:** one notification per planet/body lists its rings, commodities, hotspot counts and evidence. Later findings update the card without another popup.
- **Unified notification settings:** HGE, mining, Exobiology and Powerplay share app/game/Both/off delivery and 3/5/8-second preferences. App-only is the default; game overlay remains experimental.
- **Quieter feedback:** Exobiology notices are green. Routine Powerplay merits, route recalculation and destination-arrival notices are silent; findings and supported potential-world notices remain.
- **Powerplay intelligence:** optional separately consented EliteHub Vault reports with explicit coverage, source age and unknown-data labels.

Existing Explorer, Exobiology, fleet, engineering, material, mining and market features remain combined in the stable application.

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

1. Download **FrameShift.Command_0.10.1_x64-setup.exe** from this repository's release assets.
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
- EDSM, Spansh, Canonn, EliteHub Vault and on-demand AI features require their respective consent.
- Canonn biology lookups are off by default and send only the current system name/address, not your Commander name or journals.
- AI Search is optional, requires your API key and separate sharing consent, and can incur provider charges. Windows Credential Manager stores the key.
- Software-update requests do not upload Commander records or journals.
- Production and the combined Preview app have separate data directories. Preview notes/preferences are not automatically copied into stable v0.10.1.
- Use **Export SQLite backup** before replacing data or downgrading. Close the app before restoration and retain the original data until recovery is verified.

## Evidence and current limitations

HGE candidates are predictions, not guaranteed signals or material drops. Mining and market reports depend on provider coverage and source age.

Exobiology estimates separate base values from a conditional first-logged bonus scenario. First footfall and bonus eligibility remain unverified; recorded journal sales are confirmed earnings. Unsupported species/variant rules and missing environmental inputs remain unknown.

Powerplay retains journal and local observations, with optional separately consented EliteHub Vault reports. Provider coverage and null controllers remain explicit. No full cascade forecasts or unavailable vulnerability metrics are invented.

Packaged Windows tests cover application notifications, persistence and grouping. The optional game overlay remains experimental: actual-game foreground/fullscreen and physical multi-monitor behavior require live-game acceptance. Paid AI execution remains unverified.

## Release verification

v0.10.1 passed TypeScript validation, **464 frontend tests, 80 Rust tests and 135 browser tests**, plus packaged Windows notification and persistence checks. An isolated real v0.10.0-to-v0.10.1 upgrade preserved balances, inventory, ships, preferences and journal offsets. The v0.10.0 updater detected and signature-verified the official v0.10.1 download; v0.10.1 correctly reports itself up to date.

Installer SHA-256:

```text
3BCEF9C431B454DC5627391079B0E7E005069C130881AC6A7E306015C32E0E6D
```

## About this repository

This is the **public stable distribution repository**. Releases contain the Windows installer, its detached updater signature and `latest.json`. Application source stays private; no journals, databases, API keys or signing secrets are distributed here. Stable private source uses `master`; shared development/testing uses one `preview` branch.

Elite Dangerous and associated game assets belong to Frontier Developments. FrameShift Command is an independent companion app. Bundled artwork is illustrative.
