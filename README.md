# Lunar Phase JSON API

## Endpoint

```
https://printfn.github.io/lunar-phase/api/lunar-phase-data/{year}/index.json
```

`{year}` can be any year between `1700` and `2082` (inclusive).

The response is in this format:

```js
[
    { "Date": "1700-01-05T10:30:00", "Phase": 2 },
    { "Date": "1700-01-12T03:34:00", "Phase": 3 },
    // ...
]
```

All timestamps are in UTC.

Phases:

| ID | Name |
| --- | --- |
| 0 | New Moon |
| - | Waxing Crescent |
| 1 | First Quarter |
| - | Waxing Gibbeous |
| 2 | Full Moon |
| - | Waning Gibbeous |
| 3 | Last Quarter |
| - | Waning Crescent |

---

Based on [github.com/CraigChamberlain/moon-data](https://github.com/CraigChamberlain/moon-data)
