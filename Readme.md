# Nexium 3.14

Nexium is a pre-built OSINT multitool for Windows, designed for gathering public information. This version is already compiled as an executable (`nexium.exe`) and ready to use.

## Features

1. **Image Metadata Viewer**

   * Extracts EXIF and basic information from images (local or URL).

2. **Username Web Search**

   * Searches DuckDuckGo or Google for a username across the web.

3. **IP to Geo Lookup**

   * Resolves an IP address to geolocation data.

4. **Address Geocoding & Reverse Lookup**

   * Converts addresses to coordinates and coordinates back to addresses using OpenStreetMap.

5. **Discord User Lookup**

   * Fetches user profile via Discord API (optional bot token). Provides CDN avatar URL example.

## Usage

Run Nexium from Command Prompt:

```cmd
nexium.exe <command> [options]
```

### Commands

* `metadata <file>` — Image metadata viewer
* `usersearch <username> [--engine ddg|google]` — Search for a username online
* `ipgeo <ip>` — Get geolocation from IP
* `geocode <address>` — Convert address to coordinates
* `reverse <lat> <lon>` — Convert coordinates to address
* `discord <userid> [--token TOKEN]` — Discord user lookup

### Examples

```cmd
nexium.exe metadata image.jpg
nexium.exe usersearch adam --engine ddg
nexium.exe ipgeo 8.8.8.8
nexium.exe geocode "1600 Amphitheatre Parkway, Mountain View, CA"
nexium.exe reverse 37.422 -122.084
nexium.exe discord 123456789012345678 --token YOUR_BOT_TOKEN
```

## Notes

* Always run from CMD to see output and prevent the window from closing automatically.
* Have Fun..
