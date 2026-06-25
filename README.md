[README.txt](https://github.com/user-attachments/files/29351582/README.txt)
National School Enrollment Atlas prototype

Files included:
- index.html: patched GIS-first version of the CCD Enrollment Web Tool.
- json/geo/schools_2425_ST.geojson: state-level public school point files converted from the NCES/EDGE 2024-2025 public school geocode shapefile.

Keep your existing files in the same structure expected by the app:
- json/directory/ccd_sch_directory_2425_ST.json
- json/membership/ccd_sch_membership_1617_ST.json through ccd_sch_membership_2425_ST.json

How it works:
1. Select a state.
2. The app loads the state school directory and the matching school geography file.
3. Click a school point on the map to switch to the selected school and update the enrollment chart, KPIs, and grade table.
4. Search/load a district to zoom the map to that district's schools.

Notes:
- The app uses Leaflet and OpenStreetMap tiles from CDNs.
- The shapefile has been converted to state-level GeoJSON files for browser performance.
- Trend coloring is scaffolded; currently selected district/school highlighting is active. Full growth/decline symbology can be added once state-level enrollment summaries are precomputed.
