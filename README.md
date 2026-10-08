# Petr Nikeska

computer vision and geospatial engineer in the czech republic. mobile mapping, LiDAR, GeoAI. at CEDA Maps i turn street-level survey data (360° imagery, GNSS, LiDAR) into a map-ready inventory of traffic signs and road defects. i like the part where geospatial work stops being a notebook and starts being something that runs.

MSc geoinformatics at Palacký University Olomouc, on Erasmus+ at AUTh Thessaloniki until february 2027. open to computer vision and geospatial roles across europe after that, remote or Olomouc-shaped. the [portfolio](https://petrmikeska.cz/) has case studies and a CV.

## things i built because i wanted to

- [roundabout-exit-detection](https://github.com/MetrPikeska/roundabout-exit-detection) is YOLOv8 + ByteTrack over 5 minutes of aerial footage of an intersection in Kopřivnice. 11 ground control points from the ČÚZK orthophoto give a homography with 0.51 m mean reprojection error, so the tracks come out as GeoPackage and GeoTIFF you can drop straight into QGIS: 142 trajectories, speeds, exit counts, an O/D matrix.
- [medpz-geoai](https://github.com/MetrPikeska/medpz-geoai) detects vehicles in four 10 cm/px orthophotos of Olomouc with YOLOv8-OBB and SAHI tiling, then joins them to 14,458 RÚIAN address points through Voronoi zones to get cars per resident, and clusters the leftovers with DBSCAN to find parking lots.
- [park-accessibility-toolbox](https://github.com/MetrPikeska/park-accessibility-toolbox) is my bachelor's thesis as an ArcGIS Pro toolbox: network dataset, walking isochrones, population within reach of a park, following the European Commission's "A short walk to the park?" methodology.
- [geote-klima-ui](https://github.com/MetrPikeska/geote-klima-ui) is a web front end over a PostGIS climate database, comparing the 1961–1990 and 1991–2020 normals against projections to 2050 for czech administrative units. [live](https://geote-klima-ui.vercel.app).
- [pirati-volebni-atlas](https://github.com/MetrPikeska/pirati-volebni-atlas) maps GWR results of the 2025 parliamentary election down to municipality level, with demographics alongside and a draw-your-own-polygon tool for ad hoc aggregates. [live](https://pirati-volebni-atlas.vercel.app).
[geo-places-quiz](https://github.com/MetrPikeska/geo-places-quiz), and ESP32 sensor projects that mostly exist so the flat has numbers on a dashboard.

## the work i can't link

the CEDA Maps repos are private, so descriptors instead of code. the piece i'd show first: photogrammetric localization of traffic signs from a YOLO bbox and a GPS trajectory, around 400 commits since july 2026. position comes out as distance ⊕ bearing, the forward-facing camera is geometrically degenerate for depth, and off-axis observations are the only lever i could actually verify. LiDAR stays out of the estimate on purpose, it is the independent measuring stick. next to that: a clustering prototype that merges repeated road defect detections from several fleet vehicles into single road events, and the training set for a sign classifier (filtering, labeling, image quality scoring, duplicate removal across survey drives).

[VečerkaPlus](https://vecerkaplus.cz/) is the other half. late-night drinks and snacks delivery in Frýdek-Místek that i co-founded in april 2025: shop, operator admin and courier app, delivery zones and pricing from spatial analysis, 1,059 commits since march 2026. i also do the purchasing and run the couriers, which is a different kind of debugging.

my master's thesis compares cartographic output from ChatGPT, Claude, Gemini, Mistral and Copilot against ordinary GIS workflows. private until it is defended. before CEDA i did remote sensing at SkyMaps Geomatics: soil productivity maps, GDAL orthophoto automation, NDVI statistics for fertilizer field trials. since 2023 i also keep [olomouckymajales.cz](https://olomouckymajales.cz/) and [meetup.upol.cz](https://meetup.upol.cz/) alive through their traffic peaks.

Python, PyTorch, YOLO, OpenCV, COLMAP, GeoPandas, PostGIS, GDAL, PDAL, QGIS, FastAPI, TypeScript, Docker. reach me at piter.mikeska@gmail.com, on [LinkedIn](https://www.linkedin.com/in/mikeskapetr), or through the [portfolio](https://petrmikeska.cz/).
