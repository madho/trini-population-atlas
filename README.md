# Trini Population Atlas

Interactive data explorer for Trinidadian and Tobagonian ancestry across U.S. ZIP Code Tabulation Areas.

## Included

- Ranked population and local-share views
- Search, sorting, row details, and margin-of-error display
- Zoomable U.S. heatmap using Leaflet and Leaflet.heat
- 2024 ZCTA representative coordinates from the Census Gazetteer file
- Derived ACS 2020–2024 5-Year data in CSV format

## Run locally

```bash
python3 -m http.server 4173
```

Then open <http://127.0.0.1:4173/>.

## Data provenance

The population estimates come from U.S. Census Bureau ACS 2020–2024 5-Year Detailed Table B04006, People Reporting Ancestry. The heatmap coordinates come from the Census 2024 ZCTA Gazetteer File. Human-readable city/state labels are joined from GeoNames postal-code data; ZIP-to-place naming can reflect USPS postal conventions rather than municipal boundaries.

Relevant source links:

- https://data.census.gov/table/ACSDT5Y2024.B04006
- https://www2.census.gov/programs-surveys/acs/summary_file/2024/table-based-SF/data/5YRData/acsdt5y2024-b04006.dat
- https://www2.census.gov/geo/docs/maps-data/data/gazetteer/2024_Gazetteer/2024_Gaz_zcta_national.zip
- https://download.geonames.org/export/zip/US.zip

ACS values are statistical estimates and should not be treated as exact enumeration. The margin of error is retained in the data and shown in the explorer.
