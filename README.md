# Petr Mikeska

**Computer Vision & Geospatial Engineer** · Mobile mapping, LiDAR, GeoAI  
MSc Geoinformatics student, Palacký University Olomouc · currently on Erasmus+ at AUTH, Thessaloniki

I build computer vision and geospatial tools for mobile mapping. At [CEDA Maps](https://www.ceda.cz/) I work on a GeoAI pipeline that turns street-level survey data (360° imagery, GNSS, LiDAR) into a map-ready inventory of traffic signs and road defects. My part connects the two sides: YOLO detections, monocular depth and structure-from-motion on one, georeferencing and LiDAR validation on the other.

Besides that I co-founded [VečerkaPlus](https://vecerkaplus.cz/), a late-night delivery service in Frýdek-Místek, where I wrote the whole platform and run day-to-day operations.

🌐 [petrmikeska.cz](https://petrmikeska.cz/) · 💼 [LinkedIn](https://www.linkedin.com/in/mikeskapetr) · ✉️ piter.mikeska@gmail.com

## Selected work

**[Vehicle detection from orthophotos](https://github.com/MetrPikeska/medpz-geoai)**
YOLOv8s-OBB with SAHI tiling over four 10 cm/px orthophotos of Olomouc (EPSG:5514), combined with RÚIAN address points, Voronoi zones and DBSCAN to get vehicles per resident and to find parking lots.

**[Park Accessibility Toolbox](https://github.com/MetrPikeska/park-accessibility-toolbox)**
Bachelor's thesis: QGIS and Python toolbox measuring pedestrian access to urban green space through network analysis. [Thesis page](https://geoinformatics.upol.cz/dprace/bakalarske/mikeska25)

**[GeoteKlima UI](https://github.com/MetrPikeska/geote-klima-ui)**
Web interface over a PostGIS climate database: spatial queries and visualization of climate indices for the Czech Republic.

**[Roundabout exit detection](https://github.com/MetrPikeska/roundabout-exit-detection)**
YOLOv8 tracking with Shapely ROI polygons and a state machine that counts which exit each vehicle takes, aggregated per minute to CSV.

**[VečerkaPlus Analytics](https://github.com/MetrPikeska/vecerkaplus-analytics)**
Streamlit app on my own Ubuntu server reading the production Supabase database: sales, margins, order timing and basket analysis that drive purchasing and pricing.

**[Ski Cam Analytics](https://github.com/MetrPikeska/ski-cam-analytics)** · **[Cemetery Passport](https://github.com/MetrPikeska/cemetery-passport)** · **[DEM Terrain Analyzer](https://github.com/MetrPikeska/dem-terrain-analyzer)**
People counting from an HLS stream (YOLO ONNX on CPU), a PostGIS and Leaflet editor for cemetery records, and A* least-slope routing over a DEM.

## Stack

| | |
|---|---|
| **Spatial** | PostGIS · QGIS · ArcGIS Pro · GDAL/OGR · GeoPandas · Leaflet · MapLibre |
| **Vision & ML** | PyTorch · YOLOv8/OBB · SAHI · OpenCV · monocular depth · COLMAP |
| **LiDAR & 3D** | PDAL · Open3D · CloudCompare · Blender |
| **Code & data** | Python · TypeScript · SQL · FastAPI · PostgreSQL · Supabase · Streamlit |
| **Infra** | Git · Docker · CUDA · Vercel · self-hosted Ubuntu |
| **Hardware** | ESP32 · Arduino · C++ · sensors and home lab networking |

## Now

- Traffic sign geolocation and LiDAR-based accuracy checks at CEDA Maps
- Master's thesis on AI-generated cartography: benchmarking LLM map output against GIS workflows
- Erasmus+ semester at Aristotle University of Thessaloniki, Rural & Surveying Engineering
- Open to computer vision and geospatial engineering roles across Europe
