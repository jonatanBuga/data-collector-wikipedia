# Project Name: Wikipedia Given names and Surnams Data Collector

## Overview
This project is a data collection tool that extracts information from Wikipedia pages containing first and last names. It utilizes the Wikidata API to fetch additional data based on a unique identifier for each name. The collected data is stored in a single data frame with categorical values, making it easy to analyze and use for various applications.

## Table of Contents
1. [Introduction](#introduction)
2. [Installation](#installation)
3. [Usage](#usage)
4. [Data Collection Process](#data-collection-process)
5. [Data Frame Structure](#data-frame-structure)
6. [License](#license)

## Introduction
The Wikipedia Names Data Collector is a Python-based tool designed to gather information related to first and last names from Wikipedia pages. The collected data is enriched using the Wikidata API, which provides detailed information based on the unique identifier associated with each name.

## Installation
To use this tool, follow these steps:
1. Clone the repository to your local machine.
2. Ensure you have Python 3.x installed.
3. Install the required dependencies using the following command:
   ```
   pip install pandas wikipedia-api
   ```

## Usage
1. First, ensure you have completed the installation steps mentioned above.
2. Run the `Data_collection.py` script, which initiates the data collection process.
3. The tool will scrape Wikipedia pages to gather names and corresponding unique identifiers.
4. It will then use the Wikidata API to collect additional data based on the unique identifiers.
5. The data will be stored in a single data frame with categorical values.

## Data Collection Process
The data collection process comprises the following steps:
1. Fetching Wikipedia pages containing first and last names.
2. Extracting names from these pages.
3. Using the unique identifier associated with each name to retrieve additional data from Wikidata.

## Data Frame Structure
The collected data is stored in a pandas data frame with the following columns:

| Column Name | Description |
|-------------|-------------|
| `label` | name extracted from the Wikipedia page. |
| `Wikidata ID` | Unique identifier associated with each name on Wikidata. |
| `English Description` | English Description extracted from the Wikidata page. |
| `Language` | Language extracted from the Wikidata page. |
| `Wiki Short Lang` | Wiki Short Lang extracted from the Wikidata page. |
| `Entry` | Entry extracted from the Wikidata page. |

Please note that not all fields may be available for every name, so some cells may contain NaN values.

## License
This project is licensed under the [MIT License](LICENSE). Feel free to modify and use it according to the terms of the license.

**Note:** The Wikipedia Names Data Collector tool is not affiliated with Wikipedia or Wikidata. It is an independent project for educational and research purposes. Please make sure to use it responsibly and follow the terms of service of the respective platforms when scraping data.
