---

# Kitsap Transit – Bay Data

Bay assignment for bus pickups
  (3/25/26 - currently limited to Bremerton Transit Center (BTC))
  (stop_id = 1)

## Source
Kitsap Transit GTFS data feed cross referenced against planner run card assignments 

## Service Period
| Field | Date |
|---|---|
| Start Date | March 15, 2026 |
| End Date | June 6, 2026 |

## File
`btc_bay.json` — 509 records in JSON format and available at:
https://raw.githubusercontent.com/rebeccasc-kitsaptransit/data/main/bay/kt_trips_bay_n509.json


## Fields
| Field | Description |
|---|---|
| `block_id` | The block identifier for the vehicle assignment |
| `trip_id` | Unique trip identifier |
| `service_id` | Service pattern identifier (e.g. weekday, Saturday, Sunday) |
| `stop_id` | Stop identifier — all records in this file are stop `2` (BTC) |
| `arrival_time` | Scheduled arrival time at BTC |
| `departure_time` | Scheduled departure time from BTC |
| `route_id` | Route identifier |
| `start_date` | First date this schedule is valid |
| `end_date` | Last date this schedule is valid |

## Notes
- Records currently scoped to BTC (stop_id `1`) only
- Times are in `HH:MM:SS` format
- Dates are in `YYYY-MM-DD` format
  - xxx70 serviceID = 4   -- saturday service
  - xxx80 serviceID = 1  -- sat / sunday service
- Where a single bay assignment is not available due to timing constraints, a range of 7-9 is assigned,
  - Warning: this value instantly converts to Jul-9 in Excel.
 
