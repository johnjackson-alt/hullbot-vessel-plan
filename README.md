# Hullbot Vessel Plan

Interactive 3D vessel model for the SRV team: hull parts, cleaning zones, deployment points, deck tasks and the clean track calculator. The whole app is the single file `index.html`.

## Open it for a specific vessel

Add the vessel's particulars to the page address:

```
https://<username>.github.io/hullbot-vessel-plan/?imo=1234567&name=VESSEL%20NAME&loa=183&beam=32.2&draft=11&berth=Port%20Botany&side=port
```

| Parameter | Meaning | Required |
|---|---|---|
| `loa` | Length overall, metres (20 to 400) | Yes |
| `beam` | Beam, metres (4 to 70) | Yes |
| `draft` | Design draught, metres (1 to 25) | Yes |
| `name` | Vessel name shown on the bow and stern | No |
| `imo` | IMO number (ignored if the check digit is wrong) | No |
| `berth` | Berth name | No |
| `side` | Side alongside the quay: `port`, `starboard` or leave out for at anchor | No |

Spaces in names are written as `%20`. Without `loa`, `beam` and `draft` the page opens the standard 183 m model.

## Embed in Notion

On the vessel's Notion page type `/embed`, paste the address with that vessel's parameters, and resize the block.
