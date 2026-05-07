# Bocconi-MSc.-Thesis-Data-work

This repository contains all the data-work completed while writing my thesis titled "Strategic Selection or Patent Quality? Evidence from PTAB Trial Proceedings on the Role of Firm Size Asymmetries and Examination Leniency" for the MSc. in Economics and Social Sciences in Bocconi University. The data used was downloaded on 2nd of January 2026. For this project, I specifically use the "application_data" file within the PatEx. I also utilize the Orbis database to gain information about the firms participating in the proceedings.

## Datasets
This project uses 2 original datasets and benefits from one database. The datasets are "PTAB Trial Proceedings Data" and "Patent Examination Research Dataset (PatEx)", both downloaded from the Open Data Portal within the USPTO website. On 2nd of January 2026, there were around 19,000 proceedings. PatEx application data originally contains 14 million entries, but I only consider the examinations after December 1997 which reduces the number of entries to 11 million. After I select the participants of proceedings, I create lists to match them to the firms recorded in Orbis.

When this thesis was written, Proceedings Data required identification and a personal API key to download the dataset automatically by web scraping rather than manually downloading every 100 proceedings. PatEx did not require this as it is already in the form of a structured database, however a recent message from USPTO states that it will require having a USPTO account starting from 18th of June 2026. Orbis requires payment for full access however I was able to benefit from the subscription of Bocconi to have free access, which I am grateful for.

https://data.uspto.gov/ptab/trials/proceedings
https://data.uspto.gov/bulkdata/datasets/ecopair?fileDataFromDate=2015-12-02&fileDataToDate=2023-09-26

## Notebooks

The project consists of several Jupyter Notebooks, each one of them work on a specific dataset.

The first notebook runs the code that downloads the proceedings data using API key.
The second notebook modifies the proceedings data.
The third notebook modifies the application data.
The fourth notebook merges the two datasets above.
The fifth notebook merges the matching from Orbis with above dataset.
