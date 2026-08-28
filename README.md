# TechStreamTV

**Personal Media Streaming for Windows**

TechStreamTV is a **portable, self-hosted personal media server** for organizing, browsing, and streaming your own media library across devices on your local network.

Run TechStreamTV Server on a Windows PC, build or import your media library, and connect from browsers or compatible TechStreamTV clients across your LAN.

**No cloud media hosting. No external database server. Your library stays on your hardware.**

---

## Download

Download the latest TechStreamTV release:

[https://github.com/ablestudio-dev/TechStreamTV/releases](https://github.com/ablestudio-dev/TechStreamTV/releases)

Extract the ZIP file and run:

`TechStream.exe`

No installer or external database setup is required.

---

## Overview

TechStreamTV combines a persistent SQLite-powered media library with HTTP streaming, synchronized playback history, a responsive Web UI, and support for compatible native clients.

The TechStreamTV Server is authoritative for your library and playback state, allowing supported devices to share information such as:

- Resume position
- Watched and completed status
- Play count
- Last played
- Playback history

Pause on one supported device and continue on another.

---

## Core Features

- Persistent SQLite-powered media library
- Movies, TV series, collections, and playlists
- Stream local video files over LAN
- IPTV and M3U / M3U8 support
- Continue Watching
- Recently Added
- Most Watched
- Recently Watched
- Dynamic category discovery
- Synchronized playback progress
- Resume positions and watched status
- Play counts and playback history
- Metadata, posters, descriptions, and keywords
- TMDB metadata integration
- Responsive built-in Web UI
- Desktop, mobile, touch, and television layouts
- Remote and D-pad navigation
- Automatic LAN server discovery
- Compatible native TechStreamTV clients
- Byte-range streaming and seeking
- SRT subtitle support
- Optional multi-user authentication
- Automatic database backups and recovery
- Portable, self-contained Windows deployment

---

## Media Library

TechStreamTV uses an embedded SQLite database as the authoritative source for the active media library.

The library can store:

- Playlists and media
- Metadata and posters
- Groups and seasons
- Users and settings
- Playback history

SQLite is embedded directly into TechStreamTV and requires no separate database installation or configuration.

M3U and M3U8 remain supported for importing, exporting, IPTV, and compatibility with external applications.

---

## Library Discovery

TechStreamTV automatically generates useful discovery sections from your library and playback history.

The normal library includes:

1. Continue Watching
2. Recently Added
3. Most Watched
4. Recently Watched
5. Categories
6. Unsorted

Categories are generated from playlist keyword metadata.

Playback history can influence discovery for the current user, helping surface unwatched and less-watched content while retaining access to the complete library.

---

## Playback Sync

Playback state is maintained by TechStreamTV Server instead of being tied exclusively to one browser or playback device.

Compatible TechStreamTV clients can share:

- Resume positions
- Watched status
- Completion
- Play counts
- Last-played information
- Playback history

For example, you can begin watching something using one supported device and resume from the same position using another.

---

## Web UI

TechStreamTV includes a responsive Web UI for library discovery, browsing, and playback.

Features include:

- Horizontal discovery rows
- Continue Watching
- Recently Added
- Most Watched
- Recently Watched
- Dynamic categories
- Library Menu
- Library search
- Category filtering
- Playlist detail screens
- Posters and descriptions
- Season and collection grouping
- Resume indicators
- Watched badges
- Embedded browser playback
- IPTV / HLS playback
- Desktop and mobile layouts
- Television layouts
- Remote and D-pad navigation

Library administration remains in the TechStreamTV Server application.

---

## Native Clients

TechStreamTV Server provides the library, streaming, discovery, compatibility, and playback-state services used by compatible TechStreamTV clients.

Supported playback clients include:

- Web browsers
- TechStream Player for Windows
- TechStream Player for Android / Fire OS

Compatible native clients can automatically discover TechStreamTV servers running on the same local network.

Native clients are versioned and released independently from the Server.

---

## IPTV & M3U

TechStreamTV retains M3U and M3U8 compatibility.

Supported workflows include:

- Import M3U and M3U8 playlists
- Export library playlists to M3U
- IPTV playlists
- HTTP and HTTPS media
- Compatible HLS streams
- External playlist access for applications such as VLC

Local media uses direct HTTP streaming with byte-range support.

---

## Subtitles

TechStreamTV supports `.srt` subtitle files.

- Automatically detects matching subtitle files
- Preserves subtitle information in the media library
- Browser subtitle controls when available
- Server-provided subtitle information for compatible native clients

---

## Authentication

Optional authentication is available for shared local networks.

Features include:

- Multiple local users
- Secure password storage
- Browser session authentication
- Client authentication support
- Per-user playback history
- Per-user resume and watched state
- Per-user library discovery
- Login rate limiting

Authentication remains optional for normal private-LAN operation.

---

## Database Reliability

TechStreamTV maintains its SQLite database automatically.

Reliability features include:

- Automatic schema migration
- Write-Ahead Logging (WAL)
- Database integrity checks
- Pre-migration backups
- Rotating daily backups
- Automatic recovery from a valid backup
- Preservation of damaged databases for troubleshooting

If automatic database recovery is required, TechStreamTV informs the user.

---

## Quick Start

1. Download and extract the TechStreamTV ZIP file.
2. Run `TechStream.exe`.
3. Build or import your media library.
4. Start the server.
5. Open the Web UI from another device:

[http://YOUR-LAN-IP:5050/](http://YOUR-LAN-IP:5050/)

Compatible TechStreamTV clients can also automatically discover servers running on the same local network.

For VLC or another M3U-compatible application:

[http://YOUR-LAN-IP:5050/playlist/{id}.m3u](http://YOUR-LAN-IP:5050/playlist/{id}.m3u)

---

## Requirements

- Windows 10 or Windows 11 (64-bit)
- Devices connected to the same local network

TechStreamTV Server is self-contained and uses .NET 10 LTS.

No external database server is required.

---

## LAN & Privacy

TechStreamTV is designed around local ownership and control.

- **LAN-first** — stream directly across your local network
- **Self-hosted** — your server runs on your hardware
- **Private** — no required cloud media hosting
- **Portable** — no installer required
- **Independent** — no external database server required
- **Cross-device** — browsers and compatible clients connect directly to your server

Always use your LAN IP address when connecting from another device.

Do **not** use `127.0.0.1` from another device.

Windows Firewall may request permission for network access when TechStreamTV Server is first used.

---

## Project Direction

TechStreamTV continues to evolve as a personal media platform built around:

- Persistent media libraries
- Fast library discovery
- Cross-client playback synchronization
- Reliable native playback
- Television and remote navigation
- Server/client compatibility
- Independent but interoperable Web and native clients

The Server remains authoritative while the Web UI and native clients provide interfaces tailored to their respective platforms.

---

## License

See **LICENSE.txt** for license details.

---

**Your library. Your hardware. Your network. Your experience.**
