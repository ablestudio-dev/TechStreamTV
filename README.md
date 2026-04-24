# TechStream

Lightweight LAN Media Streaming for Windows

TechStream is a **portable, self-hosted media server** designed for simple, fast streaming of local media libraries over your network.

Stream your media to any device on your LAN using a built-in HTTP server.
No cloud. No forced accounts. No tracking. Just your media, your network.

---

## Download

Download the latest release:

[https://github.com/ablestudio-dev/techstream/releases](https://github.com/ablestudio-dev/techstream/releases)

Extract the ZIP file and run:

TechStream.exe

No installer required.

---

## Overview

TechStream turns any folder or playlist into a simple streaming source accessible from browsers, VLC, or other compatible clients.

* Runs locally on your machine
* Streams over HTTP
* Works across devices on your network
* Designed for speed and simplicity

---

## Core Features

* Stream local video files over LAN
* Built-in HTTP server (Kestrel)
* Byte-range streaming (seeking supported)
* Multiple playlists hosted simultaneously
* M3U playlist support (local + IPTV)
* Web-based playback interface
* Subtitle support (.srt)
* Optional authentication system (multi-user support)
* Portable — no installation required

---

## How It Works

1. Select a media folder or load an M3U playlist
2. Start the server
3. Connect from another device using your LAN IP

Example:

[http://YOUR-LAN-IP:5050/](http://YOUR-LAN-IP:5050/)

For VLC:

[http://YOUR-LAN-IP:5050/playlist/{id}.m3u](http://YOUR-LAN-IP:5050/playlist/{id}.m3u)

---

## Web Interface

TechStream includes a built-in web interface for:

* Browsing playlists
* Playing media directly in the browser
* Viewing server information

Accessible at:

[http://YOUR-LAN-IP:5050/](http://YOUR-LAN-IP:5050/)

---

## Playlists

TechStream supports multiple playlist modes:

### Folder Mode

* Automatically indexes media files
* Applies natural sorting

### M3U Mode

* Uses playlist order exactly as defined
* Supports IPTV and external streams

Multiple playlists can be hosted and accessed independently.

---

## Subtitles

* Automatically detects matching `.srt` files
* Loads subtitles during playback in the Web UI
* Native browser subtitle controls (CC button)

---

## Authentication (Optional)

TechStream includes an optional authentication system.

When enabled:

* Web UI requires login
* API and streaming endpoints are protected
* External clients must authenticate

Authentication is **disabled by default**.

---

## Philosophy

TechStream is built around a few core ideas:

* **LAN-first** — your media stays local
* **Portable** — no installation or system changes
* **Self-hosted** — no reliance on external services
* **Simple by default** — advanced features remain optional

---

## Roadmap Direction

TechStream is evolving into a **full media platform** built around:

* Multi-user support
* Playback tracking and resume
* Improved Web UI experience
* Multi-library and remote library support
* Cross-device compatibility

---

## Requirements

* Windows 10 or Windows 11 (64-bit)
* Devices must be on the same LAN network

---

## Notes

* Always use your **LAN IP address**
* Do **not** use `127.0.0.1` from another device
* The server binds to `0.0.0.0` for LAN access
* Windows Firewall may prompt on first run

---

## License

See **LICENSE.txt** for details.

---

Built for speed, simplicity, and full local control.
