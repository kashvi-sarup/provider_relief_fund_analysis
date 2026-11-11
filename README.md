# Provider Relief Fund Analysis

## Project Overview

This project analyzes COVID-19 Provider Relief Fund High-Impact Payments distributed to hospitals and health systems. The report examines funding distribution across recipients 
and states using publicly available data from the Health Resources and Services Administration (HRSA), 

The report focuses on:
1. Summarizing Provider Relief Fund payments to healthcare organizations.
2. Examining how payments were distributed across states.
3. Identifying the ten largest recipients of High-Impact Payments.

## Repository Structure

- `data/provider_relief_funds.csv`: Original dataset used for the analysis
- `code/make_table.R`: Code for generating the table of the top 10 recipients
- `code/make_figure.R`: Code for generating the figure showing the top 10 states by total payments
- `Final Project Report.Rmd`: Main R Markdown report containing all elements
- `Makefile`: Instructions for generating the HTML report
- `output/final_report.html`: Final HTML report

## How to Generate the Report

To reproduce the report:

1. Download or clone this repository.
2. Open the project directory in RStudio.
3. Ensure the required R packages are installed: `dplyr`, `ggplot2`, `gtsummary`, `knitr`, and `rmarkdown`.
4. Open the Terminal and run:
    make report
The report will be generated as `output/final_report.html`.

## Tables and Figures

**Required Table:** `code/make_table.R` contains the code needed to generate the table showing the top 10 recipients
**Required Figure:** `code/make_figure.R` containts the code needed to generate the figure showing the top 10 states

## Data Source
Provider Relief Fund COVID-19 High Impact Payments dataset, published by HRSA and available through data.cdc.gov.