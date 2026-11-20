# US Cable Live

Curated US cable live TV playlist (M3U) + programme guide (XMLTV), built 2026-11-20 from iptv-org's US list.

- 58 channels, each verified live that day (returned a valid .m3u8)
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

- 54 of the 58 channels have listings (9,372 programmes, Nov 19–27, 2026)
- Built from EPGTalk (Schedules Direct) and EPGShare US2, with channel IDs rewritten to match this playlist's `tvg-id`s
- No guide data exists in those sources for: Fox Weather, NBC News NOW, Hallmark Movies & More, Adult Swim

## Caveats

Many streams are unofficial mirrors from iptv-org, not official cable feeds. Expect some to die over time — re-verify before trusting any one channel for a game. Guide data is a snapshot and goes stale after about a week; rebuild it to refresh.
