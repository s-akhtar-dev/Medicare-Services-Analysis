# Medicare-Services-Analysis
![](https://pbs.twimg.com/media/GkSauOCbUAA7tJ6?format=jpg&name=medium)

# Medicare Services Analysis in R

[![R Version](https://img.shields.io/badge/R-%3E=4.0-blue.svg)](https://www.r-project.org/)
[![tidyverse](https://img.shields.io/badge/tidyverse-tidyverse-brightgreen.svg)](https://www.tidyverse.org/)

## Overview

This study analyzes a Medicare Part B 2022 dataset attained from the the Centers for Medicare & Medicaid Services (CMS) to explore Medicare data and trends. A variety of techniques were used to derive conclusions such as data manipulation, visualizations in R with `ggplot2`, and statistical analysis. 

## Project Goals

*   Apply data analytics tools using R to gain insights into Medicare data.
*   Explore, visualize, and analyze the dataset using `tidyverse` packages.
*   Communicate findings clearly and concisely through visualizations and statistical analysis.
*   Investigate specific questions related to service utilization and cost variations within the Medicare system.

## Dataset

The dataset is sourced from the Centers for Medicare & Medicaid Services (CMS):

*   **Name:** Medicare Physician & Other Practitioners - by Geography and Service
*   **Year:** 2022
*   **Size:** 42 MB
*   **Rows:** 270,673

### Links

*   [Medicare Physician & Other Practitioners - by Geography and Service Overview](https://data.cms.gov/provider-summary-by-type-of-service/medicare-physician-other-practitioners/medicare-physician-other-practitioners-by-geography-and-service)
*   [Medicare Physician & Other Practitioners - by Geography and Service Dataset](https://data.cms.gov/provider-summary-by-type-of-service/medicare-physician-other-practitioners/medicare-physician-other-practitioners-by-geography-and-service/data)
*   [Medicare Physician & Other Practitioners - by Geography and Service Data Dictionary](https://data.cms.gov/resources/medicare-physician-other-practitioners-by-geography-and-service-data-dictionary)

### Description

The dataset includes information on:

*   Medicare provider locations and services
*   Geographic factors
*   Quantitative representations of payments submitted by providers and aid paid to beneficiaries by Medicare.

Key variables include:

*   **Geographic Information:** `provider_geo_level`, `provider_geo_code`, `provider_geo_description`
*   **Service Information:** `hcpcs_code`, `hcpcs_description`, `hcpcs_drug_indicator`, `place_of_service`
*   **Utilization Metrics:** `total_providers`, `total_services`, `total_beneficiaries`, `total_beneficiary_day_services`
*   **Financial Metrics:** `average_submitted_charge`, `average_medicare_allowed_amount`, `average_medicare_payment_amount`, `average_medicare_standardized_amount`

Note: These variables were renamed for clarity.

## Main R Libraries Used

*   **tidyverse:** For data manipulation and visualization (specifically, `dplyr` and `ggplot2`)

## Setup

1.  **Install R:** Make sure you have R installed on your system.  You can download it from [The R Project](https://www.r-project.org/).
2.  **Install `tidyverse`:**

    ```
    install.packages("tidyverse")
    ```

3.  **Download the Dataset:** Download the "Medicare Physician & Other Practitioners - by Geography and Service Dataset" from the CMS website (link provided above).  Save it to a suitable directory on your computer.
4.  **Clone the Repository:** Clone this GitHub repository to your local machine.

    ```
    git clone https://github.com/s-akhtar-dev/Medicare-Services-Analysis
    ```

5.  **Set Working Directory:** In your R script, set the working directory to the location where you've stored the dataset and the R scripts.

## Usage

1.  **Load Libraries:** Load the necessary libraries at the beginning of your R script:

    ```
    suppressPackageStartupMessages(library(tidyverse))
    ```
    or
    ```
    library(tidyverse)
    ```

3.  **Load the Data:** Load the Medicare dataset into R:

    ```
    medicare <- read.csv("path/to/your/medicare_providers_2022.csv") # Replace with the correct path
    ```

4.  **Run the Analysis:** Execute the R scripts in the repository to perform the data analysis and generate visualizations.

## Acknowledgements

This study was created for Data Analytics Programming taught by Dr. Julia Olivieri. Without her support and guidance, this project would not have been possible.

