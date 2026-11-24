# ESG Country Clustering Dataset (2001–2021)

## Overview
This repository supports the study titled:

**Clustering Countries Based on ESG Metrics: A Machine Learning Approach to ESG Factors**

The study uses a country-level compilation of Environmental, Social, and Governance (ESG) indicators obtained from the World Bank. The analysis period reported by the researchers is **2001–2021**. The dataset was supplied to an ESG-based classifier prototype to examine preprocessing and clustering using K-means and Hierarchical clustering.

Countries mentioned in the study description include Afghanistan, Albania, Algeria, Andorra, Bangladesh, Côte d'Ivoire, Croatia, Cuba, Estonia, Ethiopia, Grenada, Maldives, Mali, Malta, Niger, and others.

## Repository contents
This deposit includes the original CSV files supplied for preparation of the repository:

| File | Description |
|---|---|
| `ESGCSV.csv` | Main country/aggregate-by-indicator data table. |
| `ESGCountry.csv` | Country and aggregate metadata. |
| `ESGSeries.csv` | Indicator metadata, including indicator names, definitions and source information where provided. |
| `ESGcountry-series.csv` | Country-indicator notes. |
| `ESGfootnote.csv` | Indicator and observation footnotes. |
| `ESGseries-time.csv` | Notes for selected indicator-year combinations. |
| `ESG_Indicator_Dictionary.csv` | Documentation extract derived from the supplied indicator metadata. |

## Analysis period versus source-file coverage
The research analysis period is **2001–2021**, as confirmed by the researchers. The original downloaded main CSV includes annual columns outside this period. Those additional years are part of the original source download and should not be interpreted as years included in the reported clustering experiments.

This repository package currently preserves the supplied original CSV files. It does not claim that the main CSV has already been filtered to only 2001–2021 or to the final country/indicator subset used in the experiments. If a separate analysis-ready file is deposited, it should be clearly named and documented with the exact country list, selected indicators, missing-data handling and preprocessing steps.

## Data structure
The main data file is in a wide format with country/aggregate and indicator identifiers, followed by annual value columns. Consult `ESGCountry.csv` for country/aggregate metadata and `ESGSeries.csv` for indicator definitions and source information. Blank cells represent missing or unavailable values in the supplied files.

The country metadata includes both individual economies and aggregates. Regional, income-group and other aggregate entries should not be described as sovereign countries or included in a country-only analysis without an explicit methodological reason.

## Methods context
According to the researchers' dataset description, the data were used as input to an ESG-based classifier prototype to assess preprocessing and clustering with:
- K-means clustering
- Hierarchical clustering

The repository documentation does not independently specify the final feature-selection procedure, normalization method, missing-value treatment, distance/linkage settings, optimal-cluster criterion, evaluation metrics, or economic-category comparison. These should be documented from the actual experiment/code before the repository is treated as a fully reproducible record.

## Data source and attribution
The researchers report that the data were compiled from and downloaded directly from the World Bank. The supplied files include indicator-level source and licence fields in `ESGSeries.csv`. Please cite the World Bank source and any underlying third-party providers identified in that metadata.

Before publishing, add the exact World Bank download page or dataset URL and the date on which the data were downloaded, if known. Check the reuse conditions for the data and third-party indicators before selecting a repository-wide licence. Do not assume that one licence applies to every indicator.

## Recommended citation
After publishing this record, cite it using the DOI assigned . Also cite the original World Bank dataset and any underlying sources required by the indicator metadata.

