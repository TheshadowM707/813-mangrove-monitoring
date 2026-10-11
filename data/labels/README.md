# Training labels

`canopy_polygons.geojson` (class 1) and `other_polygons.geojson` (class 0) hold the polygons used to train and test the Random Forest in `notebooks/02_main_analysis.ipynb`.

They are visual interpretation of a public sub-metre satellite basemap, drawn inside homogeneous areas away from edges. They are not field data. The not-canopy polygons cover farmland and gardens, open water, intertidal flats and algae mats, the pale lagoon inside the stand, bare sand, housing and industrial land.

**These two files must be committed**, otherwise the notebook cannot run end to end. To (re)create them, see section 5 of the notebook (paste coordinate lists, or set `DRAW_LABELS = True` and draw).

Format: GeoJSON `FeatureCollection` of `Polygon` features in EPSG:4326 (lon, lat), each with a `class` property.
