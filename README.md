# Common Utilities (EXILED)

An EXILED plugin with configurable server utilities for SCP: Secret Laboratory.

## This fork

Version **8.1.3** is an EXILED 9 compatibility build based on [ExMod-Team/Common-Utils](https://github.com/ExMod-Team/Common-Utils), itself a fork of [Exiled-Team/Common-Utils](https://github.com/Exiled-Team/Common-Utils). It updates the EXILED references, fixes compatibility issues, and preserves the upstream plugin features. Upstream authorship is retained in the code.

Compatibility changes and this README were prepared with **OpenAI Codex**. The original project and its authors remain credited to ExMod-Team and Exiled-Team.

## Features

- Configure SCP-914 role and item upgrades, effects, and teleport destinations.
- Set starting inventories and ammunition by role.
- Configure escape role changes while handcuffed, role health, health on kill, and damage multipliers.
- Adjust radio battery use, AFK handling, item and ragdoll cleanup, and warhead lighting.
- Configure round broadcasts and other server behavior exposed by the upstream plugin.

## Install

1. Download [`Common.Utilities.dll`](https://github.com/Tomut0/Common-Utils/releases/latest/download/Common.Utilities.dll).
2. Put it in your EXILED plugin directory, for example `.config/EXILED/Plugins/<port>/` on Linux.
3. Start the server. EXILED creates the plugin configuration under its `Configs/Plugins/CommonUtilities` directory.

This repository does not include any server-specific configuration.

## Compatibility

| Component | Version |
|---|---:|
| SCP: Secret Laboratory dedicated server | 14.2.9 |
| EXILED runtime | 9.15.3 |
| EXILED build reference | 9.15.2 |
| Plugin | 8.1.3 |

Runtime compatibility was confirmed in server logs on **2026-11-02** using SCP:SL 14.2.9 and EXILED 9.15.3 (test build 8.1.2). Version 8.1.3 is rebuilt from the same tested source with the plugin version metadata incremented.

## Build

Build `Common Utilities.sln` in Release configuration with .NET Framework 4.8 targeting tools and `EXILED_REFERENCES` set to the SCP:SL/EXILED reference assemblies. The output is `bin/Release/Common Utilities.dll`.

## Credits and license

- Upstream fork: [ExMod-Team/Common-Utils](https://github.com/ExMod-Team/Common-Utils)
- Original project: [Exiled-Team/Common-Utils](https://github.com/Exiled-Team/Common-Utils)
- The project build metadata declares **CC BY-SA 3.0**; see the upstream repository for its current license information.
