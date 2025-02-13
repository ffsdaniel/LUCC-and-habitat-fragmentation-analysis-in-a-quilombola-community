# Analysis of Land Use and Cover Change (LUCC) and Habitat Fragmentation

This notebook presents the methodology used in a study on the analysis of land use and cover change (LUCC) and habitat fragmentation in a traditional quilombola community in Minas Gerais, Brazil. The work was carried out using Python 3.12 and libraries such as `geopandas`, `rasterio`, `scikit-learn`, `pylandstats` and `scipy`.

## Notebook Contents
- Land Use Classification using Random Forest**
- Habitat Fragmentation Analysis
- Statistical Tests

The notebook includes the classification of eight different land uses and land covers, such as forest formations, savannas, pastures and water bodies, using Sentinel 2 multiband images and training data.

## How to use
1. Clone this repository.
3. Download the data folder.
4. Install the necessary dependencies listed in the notebook.
5. Run the notebook to reproduce the analysis.


## Repository Structure and File Description
DATA/
Contains all data files used in the project.

DNPM/
Files related to the National Department of Mineral Production (DNPM):

DNPM_INTERSECCAO.*: Shapefiles representing intersection areas with DNPM data.
REQUERIMENTO_CONCESSAO/: Subfolder containing files related to mineral concession requests.

FINAL_LUCC_RASTERS/
Final land use and land cover (LUCC) rasters:

Diferenca_Uso_de_Solo_2018_total.tif and Diferenca_Uso_de_Solo_2024_total.tif: Rasters for land use in the area occupied by outsiders between 2018 and 2024.
Pontinha_Uso_de_Solo_2018_total.tif and Pontinha_Uso_de_Solo_2024_total.tif: Rasters representing land use in the Pontinha quilombola community area for the years 2018 and 2024.
Uso_de_Solo_2018_total.tif and Uso_de_Solo_2024_total.tif: Land use rasters for the complete area for the years 2018 and 2024.

FRAGMENTATION/
Files related to habitat fragmentation analysis:

base_de_dados_patch_metrics.xlsx: Spreadsheet with fragmentation metrics for the years 2018 and 2024.
Formacoes_naturais_*.tif: Rasters representing natural formations (difference, Pontinha, and total) for 2018 and 2024.
patch_metrics_*.xlsx: Spreadsheets with specific fragmentation metrics for different areas and years.
spatiotemporalzonal_metrics.xlsx: Spreadsheet with spatiotemporal metrics.

MULTIBAND_RASTER_2018/
Multiband rasters from 2018:

Mesclado_RGB_NDVI_31983_recorte_multibanda.tif: Multiband raster (RGB + NDVI) clipped to the study area in 2018.
MULTIBAND_RASTER_2024/
Multiband rasters from 2024:

MOSAICO_RGB.tif: Multiband raster (RGB) for 2024.
MOSAICO_SRTM_NDBI_NDVI_NDWI_RGB_B8.tif: Multiband raster with vegetation indices (NDVI, NDWI) and elevation (SRTM) for 2024.


OCCUPIED_QUILOMBO_AREA_SHAPEFILE/
Shapefiles of the area occupied by the quilombola community:

Pontinha.*: Shapefiles delimiting the area occupied by the Pontinha quilombola community.

OTHER/

Other relevant files:

licenciamentos_concedidos_paraopeba.xlsx: Spreadsheet with information on licenses granted in the Paraopeba region.
ide_2101_mg_empreendimentos_licenciados_pto/: Shapefiles related to licensed enterprises in Minas Gerais.
ide_2101_mg_historico_empreendi_lic_2013_2019_pto/: Shapefiles with a historical record of licensed enterprises between 2013 and 2019.


TOTAL_QUILOMBO_AREA_SHAPEFILE/
Shapefiles of the total area of the quilombola community:

AREAIMOVEL. and Area_do_Imovel.:** Shapefiles delimiting the total area of the quilombola community from SICAR.

TRAINING_POINTS/
Training points for land use classification:

pontos_treinamento_2018_final. and pontos_treinamento_2024_final.:** Shapefiles with training points for the years 2018 and 2024, used in land use classification.


## Dependencies
- Python 3.12
- Libraries: `geopandas`, `rasterio`, `scikit-learn`, `pylandstats`, `scipy`

## Author
- **Daniel Fernandes** (2024)

## License
This project is licensed under the MIT license. See the `LICENSE` file for more details.
