# Wound Up playtest schedule

The game reads `schedule.json` (every 10 minutes) to know when playtest builds may be played.
Edit it on GitHub (open the file, click the pencil, change it, "Commit changes"). Changes reach
players within about 10 minutes, no new build needed.

- `weekly`: the regular sessions, e.g. `{ "open": "Fri 06:00", "close": "Mon 06:00" }` (US Central time).
- `extra_open`: one-off extra sessions, e.g. `{ "from": "2026-11-26T18:00:00-06:00", "to": "2026-11-26T23:00:00-06:00", "note": "Thanksgiving" }`.
- `closed`: one-off closures (beat everything else), same format.
- `kill_switch`: `true` closes the playtest for everyone right now.
- `min_build`: builds older than this label (e.g. `"playtest-2026-10-26d"`) are told to download the new one.
- `message`: a line shown on the closed screen and the title screen ("New build tonight!").
- `discord`: your invite link, for the "Join the Discord" button.
- `dev_steam_ids`: extra Steam IDs that are never locked.

Times with `-06:00` are Central Standard Time (winter), `-05:00` Central Daylight Time (summer).
