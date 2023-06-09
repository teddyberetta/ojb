# ojb: bitcoin ordinals jobs protocol

Time > money.

## Abstract

We create a protocol to post jobs as ordinals.

## Specification

`ojb` are `json` ordinals containing the following properties. `*` indicates required field.

- `title`*: `string`
- `descr`*: `string`
- `loc`
  - `lat`: `number`
  - `long`: `number`
- `prereqs`: `string`
- `reqs`: `string`
- `comp`: `string`
- `start`: `date`
- `end`: `date`
- `apply`: `date`
- `url`: `string`

## Example

```json
{
  "p": "ojb",
  "title": "Professional Softball Player",
  "descr": "Womens sports are on the rise. Become a professional female softball player today!",
  "loc": {
    "lat": 40.7128,
    "long": 74.0060
  },
  "prereqs": "> 0.300 batting average on D1 college team",
  "reqs": "50 games per year",
  "comp": "10,000 sats/game",
  "start": "2024-01-01",
  "end": "2024-12-31",
  "apply": "2023-08-31",
  "url": "https://soonersports.com/sports/softball"
}
```

## Recommendations

- Inscribe the `ojb` from a [SID](https://army-of-youth.gitbook.io/sid-protocol/) compatible wallet.
