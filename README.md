## sentinel1-sar-flood-mapping

Implementation of a Cloud-Based Sentinel-1 SAR Workflow for Flood Change Detection in Germany's Ahr Valley

This project demonstrates cloud-based Sentinel-1 SAR flood-related change detection using STAC, openEO, and Python. Sentinel-1 GRD imagery from the July 2021 Ahr Valley flood in Germany is accessed through Copernicus Data Space, validated using acquisition metadata, and processed using orbit-consistent VV backscatter measurements.

The workflow includes pre- and post-flood backscatter comparison, median filtering, connected-region analysis, ESA WorldCover-based urban change detection, and GeoTIFF export for QGIS.

### Result snapshots

[VV backscatter change](docs/results/vv_backscatter_change_db.png): Pre- and post-flood VV backscatter change map.

[VV median filter comparison](docs/results/vv_median_filter_comparison.png): Comparison of original and median-filtered VV backscatter changes.

[SAR change region filtering](docs/results/sar_change_region_filtering.png): Connected-region filtering to remove small isolated changes.

[Urban positive VV change](docs/results/urban_positive_vv_change.png): Positive VV backscatter changes within ESA WorldCover built-up areas.

[Combined flood-related SAR changes](docs/results/combined_flood_related_sar_changes.png): Combined negative VV changes and positive urban VV changes.

[Flood-related SAR urban overlay](docs/results/flood_related_sar_urban_overlay.png): Urban SAR changes visualized over satellite imagery in QGIS.

[Flood-related SAR valley overlay](docs/results/flood_related_sar_valley_overlay.png): SAR changes along the Ahr Valley visualized over satellite imagery in QGIS.

**Keywords:** Python, Sentinel-1 SAR, STAC, Copernicus Data Space, openEO, ESA WorldCover, Rasterio, NumPy, SciPy, GeoTIFF, and QGIS.

**Acknowledgment:** Sentinel-1 and ESA WorldCover data accessed through the Copernicus Data Space Ecosystem. Satellite basemap imagery provided by Esri World Imagery.
