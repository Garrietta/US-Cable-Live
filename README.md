# US Cable Live

Curated US cable live TV playlist (M3U) + programme guide (XMLTV), built 2026-11-20 from iptv-org's US list.

- 52 channels, each verified live (returned a valid .m3u8) — streaming-only news channels removed 2026-11-20 (NBC News NOW, ABC News Live, Fox Weather, AccuWeather NOW, Law & Crime, Scripps News)
- Real cable channels only: Sports, News, Entertainment, Kids, Spanish
- No Pluto FAST single-show / throwback playlist channels, no local affiliates
- Hoosiers coverage: Big Ten Network, ESPN, ESPN2, ESPNU, FS1, ABC

## Use it

In Nuvio / Nuvio ReSeq: Live TV → Settings → IPTV Playlists → Add M3U Playlist, paste:

```
https://raw.githubusercontent.com/Garrietta/US-Cable-Live/main/US-Cable-Live.m3u
```

The guide is linked in the playlist header (`x-tvg-url`), so Nuvio loads it by itself — no separate EPG step. The guide file is also available directly:

```
https://raw.githubusercontent.com/Garrietta/US-Cable-Live/main/US-Cable-Live-EPG.xml
```

## Guide

- 51 of the 52 channels have listings (9,145 programmes, Nov 19–27, 2026)
- Built from EPGTalk (Schedules Direct) and EPGShare US2, with channel IDs rewritten to match this playlist's `tvg-id`s. Adult Swim has no separate guide feed anywhere — its listings are Cartoon Network's 5pm–6am ET block (22:00–11:00 UTC), sliced out of Cartoon Network's guide
- No guide data exists in those sources for: Hallmark Movies & More (only channel without listings)

## Caveats

Many streams are unofficial mirrors from iptv-org, not official cable feeds. Expect some to die over time — re-verify before trusting any one channel for a game. Guide data is a snapshot and goes stale after about a week; rebuild it to refresh.
