# Paraguay Import Export Data MCP

**Paraguay Customs Data: Importers, Suppliers & HS Codes.** Paraguay import export data for your AI assistant. Search Paraguay customs shipment records, find importers and foreign suppliers, and break down trade by HS code, partner country and counterparty company, through the Model Context Protocol.

An AI-native alternative to Paraguay trade data from Panjiva, ImportGenius, Volza, Seair, TradeInt and ExportGenius: ask in plain language instead of exporting spreadsheets.

The MCP connection is provided by [The Company Atlas](https://thecompanyatlas.com). This repository does not run a separate server.

## Connect

```
https://thecompanyatlas.com/mcp/trade/paraguay
```

Add this URL as a custom MCP connector in Claude, ChatGPT, Cursor, or any MCP-compatible client. Sign in with Google when prompted.

- Transport: Streamable HTTP
- Auth: Google OAuth (sign in once, stays authorized)
- Free accounts get 50 credits per calendar month
- Defaults to Paraguay: the server tells your AI to filter on `PY` unless you ask about another country

## Paraguay data coverage

- **Years:** 2024–2026
- **Records:** Import declarations: Paraguayan importer, foreign supplier, origin country, HS code, goods description, value, quantity, port and date.
- **Country code:** `PY` (use `buyerCountry: "PY"` for imports into Paraguay)
- **Common products:** refined fuel (HS 2710), cars (HS 8703), fertilizers (HS 3105), phones (HS 8517)

## Notable traders in the data

Companies that appear most often in recent Paraguay records (by number of declaration lines, not value):

**Importers**

- Puma Energy Paraguay
- Petróleos Paraguayos (Petropar)
- Monaco Comercial Import Export
- Barcos y Rodados
- Petróleos del Sur
- Monte Alegre

## Example prompts

- *"Who are the top importers of fertilizers (HS 3105) into Paraguay?"*
- *"Which suppliers ship fuel to Petropar?"*
- *"What does Monaco Comercial Import Export import, by HS code?"*
- *"List Paraguayan importers of cars (HS 8703) in 2025"*
- *"Show recent import shipments for Barcos y Rodados"*

## Tools

### Trade search

| Tool | Description |
|---|---|
| `Trade_search_trades` | Paginated customs shipment search: filter by HS code, buyer, seller, country, port, value and date range |
| `Trade_company_trade_volume_by_year` | Rank importers or exporters by declared value and line counts per year, with HS code and country filters |

### Trade analytics

| Tool | Description |
|---|---|
| `Trade_hs_code_breakdown` | For one company, import and export value by HS chapter, heading or subheading |
| `Trade_year_country_breakdown` | For one company, trade value by year and counterparty country |
| `Trade_partner_breakdown` | For one company, trade value by year and matched counterparty company |

### Company registry

| Tool | Description |
|---|---|
| `Company_search` | Search the global company registry by name or id, with optional country filter |
| `Company_get_by_id` | Full company profile by id |

## Keywords

Paraguay import data, Paraguay export data, Paraguay customs data, Paraguay shipment data, importers in Paraguay, Paraguay buyers and suppliers, HS code search, datos de importación Paraguay, importadores de Paraguay, comercio exterior, NCM
