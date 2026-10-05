# 14DayLauncher

14DayLauncher is a Windows desktop launcher for the 14Day private multiplayer server and its modpack.

## Purpose

The launcher provides participating players with a simple way to:

- Sign in using their own Microsoft account.
- Authenticate their Minecraft Java Edition account.
- Retrieve their Minecraft profile, including username and UUID.
- Install and maintain the required game, Forge, mods, configuration files, and resource packs.
- Launch the correct game configuration for the 14Day multiplayer server.

## Authentication

14DayLauncher uses the standard Microsoft authentication flow.

The authentication process is:

Microsoft Account → Xbox Live → XSTS → Minecraft Services → Minecraft Profile

14DayLauncher does not collect Microsoft account passwords.

Authentication is performed through Microsoft's authentication system, and the launcher is implemented as a public desktop client without a client secret.

## Minecraft Services API Usage

Minecraft Services API access is required to:

1. Exchange an authenticated XSTS token for a Minecraft access token.
2. Retrieve the authenticated user's Minecraft Java Edition profile.
3. Obtain the legitimate player's username and UUID before launching the game.

14DayLauncher does not bypass authentication, ownership, licensing, entitlement, or security checks.

Users must authenticate using their own Microsoft account and must have legitimate access to Minecraft Java Edition.

## Platform

- Windows desktop application
- Electron
- Minecraft Java Edition
- Minecraft 1.20.1
- Forge 47.4.10

## Project Status

14DayLauncher is currently under development for use with the 14Day multiplayer server.
