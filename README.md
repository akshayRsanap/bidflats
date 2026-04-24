# BidFlats - Bank Auction Properties India

Live web platform for SARFAESI bank auction properties across India.

**Live site:** https://akshayrsanap.github.io/bidflats/

---

## Features

- Real listings from IBAPI (ibapi.in) - 9000+ live properties
- Search by city, price, property type, bank
- Live auction countdown timers
- Grid + interactive map view (Leaflet.js)
- Property detail modal: EMI calc, legal info, direct bidding link
- Favorites panel, discount badges, mobile responsive

---

## Data Source

Listings scraped from **ibapi.in** (Indian Banks Auctions portal,
an IBA initiative under Ministry of Finance). 9000+ live properties.

---

## Running the Scraper



The scraper writes . Open  - it auto-loads
from  if present, otherwise shows 16 sample listings.

### Flags

| Flag | Default | Description |
|------|---------|-------------|
| --states | MH KA DL TN GJ TS | State codes |
| --types | P1 | P1=Residential P2=Commercial |
| --limit | 100 | Max properties |
| --all | off | Fetch all (ignores --limit) |
| --no-detail | off | Skip detail API (faster) |
| --output | properties.json | Output filename |
| --delay | 0.4 | Seconds between API calls |

---

## Tech Stack

- Vanilla HTML/CSS/JS, no build step
- Leaflet.js + OpenStreetMap for maps
- Python 3 stdlib scraper (no pip needed)
- IBAPI ASP.NET WebMethod API (reverse-engineered)

---

## Structure


