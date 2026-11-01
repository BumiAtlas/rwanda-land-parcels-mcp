# Rwanda Land Parcels & UPI Lookup MCP

Connect your AI assistant (Claude, ChatGPT, Cursor) to [BumiAtlas](https://bumiatlas.com) for Rwandan land research through the Model Context Protocol (MCP).

This listing is a focused entry point for:

- All of Rwanda's ~11.7M registered parcels from the National Land Authority's Land Administration Information System (LAIS), from the 2009–2013 systematic registration
- Parcel lookup by UPI (`1/02/09/02/9430`: province/district/sector/cell/parcel), by district, sector, cell and village (paged), or coordinates
- Recorded area and the parcel's province, district, sector, cell and village
- Satellite and street map images of a parcel and its neighbours, labelled by parcel number

Parcels have no owner, title or price information.

## Connect

```
https://bumiatlas.com/mcp/rwanda
```

Add it as a custom connector in any MCP client and sign in with Google. Tools, examples and data notes: [bumiatlas.com/mcp-docs/rwanda](https://bumiatlas.com/mcp-docs/rwanda).

- **Claude:** Settings → Connectors → Add custom connector, paste the URL, then Connect.
- **ChatGPT:** Settings → Apps & Connectors → Advanced → Developer mode, then Create with the URL and OAuth authentication.

## Tools

| Tool | Description |
|---|---|
| `RW_parcel_search` | Find parcels by UPI, by district (sector, cell, village; paged), or by `latitude, longitude`; each result is the whole record, the boundary as GeoJSON on request |
| `RW_parcel_image` | Satellite or street map image of a parcel or point, with every parcel in view outlined and labelled with its parcel number |

## Example prompts

- *"Which parcel is at -1.9441, 30.0619? What is its UPI?"*
- *"Look up UPI 1/02/09/02/9430 and show it on satellite imagery."*
- *"List the parcels in Kimironko sector, Gasabo."*
- *"How large is this parcel?"*

## Data source

Parcels © National Land Authority (NLA) of Rwanda, Land Administration Information System (LAIS), via geodata.rw. A copy of public data for research, not a legal land record.
