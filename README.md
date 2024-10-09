# README

# Considering Bias in Data

## Project Goal

This homework explores the concept of bias in data using Wikipedia articles. It combines a dataset of Wikipedia articles with a dataset of country populations and uses a machine learning service called ORES to estimate the quality of each article.

Then, it analyzes  how the coverage of politicians on Wikipedia and the quality of articles about politicians varies among countries.

## Source Citation

The Wikipedia Category:Politicians by nationality was crawled to generate a list of Wikipedia article pages about politicians from a wide range of countries. This data is saved as **politicians_by_country.AUG.2024.csv**

The population data is available in CSV format as **population_by_country_AUG.2024.csv** This dataset was downloaded from the world population data sheet published by the Population Reference Bureau.


## License of Source Data



## License of Source Code

# Article Page Info MediaWiki API Example
This example illustrates how to access page info data using the [MediaWiki REST API for the EN Wikipedia](https://www.mediawiki.org/wiki/API:Main_page). This example shows how to request summary 'page info' for a single article page. The API documentation, [API:Info](https://www.mediawiki.org/wiki/API:Info), covers additional details that may be helpful when trying to use or understand this example.

## License
This code example was developed by Dr. David W. McDonald for use in DATA 512, a course in the UW MS Data Science degree program. This code is provided under the [Creative Commons](https://creativecommons.org) [CC-BY license](https://creativecommons.org/licenses/by/4.0/). Revision 1.2 - September 16, 2024

# Requesting ORES scores through LiftWing ML Service API
Wikimedia Foundation (WMF) is reworking access to their APIs. It is likely in the coming years that all API access will require some kind of authentication, either through a simple key/token or through some version of OAuth. For now this is still a work in progress. You can follow the progress from their [API portal](https://api.wikimedia.org/wiki/Main_Page). Another on-going change is better control over API services in situations where those services require additional computational resources, beyond simply serving the text of a web page (i.e., the text of an article). Services like ORES that require running an ML model over the text of an article page is an example of a compute intensive API service.

Wikimedia is implementing a new Machine Learning (ML) service infrastructure that they call [LiftWing](https://wikitech.wikimedia.org/wiki/Machine_Learning/LiftWing). Given that ORES already has several ML models that have been well used, ORES is the first set of APIs that are being moved to LiftWing.

This example illustrates how to generate article quality estimates for article revisions using the LiftWing version of [ORES](https://www.mediawiki.org/wiki/ORES). The [ORES API documentation](https://ores.wikimedia.org) can be accessed from the main ORES page. The [ORES LiftWing documentation](https://wikitech.wikimedia.org/wiki/Machine_Learning/LiftWing/Usage) is very thin ... even thinner than the standard ORES documentation. Further, it is clear that some parameters have been renamed (e.g., "revid" in the old ORES API is now "rev_id" in the LiftWing ORES API).


## License
This code example was developed by Dr. David W. McDonald for use in DATA 512, a course in the UW MS Data Science degree program. This code is provided under the [Creative Commons](https://creativecommons.org) [CC-BY license](https://creativecommons.org/licenses/by/4.0/). Revision 1.0 - August 15, 2023



## Summary of Terms of Use



## Intermediary and Final Data Files/Schema

The following contextual files are either generated upon creation of the repository or loaded in/duplicated:

1.  **README.md** Created in R
2.  **LICENSE.txt**
3.  **wp_pages_info_example.ipynb** Example source code provided via course materials
4.  **wp_ores_liftwing_example.ipynb** Example source code provided via course materials
5.  **politicians_by_country.AUG.2024.csv** Source data - politicians by country, taken from Wikipedia
6.  **population_by_country_AUG.2024.csv** Source data - world population data sheet published by the Population Reference Bureau.

The following intermediary data files are generated by the scripts in this repository:


The following final data files are generated by the scripts in this repository:


## Known Issues and Considerations


## Reproducibility and Citation

This homework follows reproducible research practices. Portions of the code has been text-generated by ChatGPT, OpenAI, 14 Oct. 2024. These portions are noted in the markdown of the code preceding them, including the prompt, and are wrapped in a function to contain them. Note that all portions of text-generated code have been edited from their original versions for logic, clarity, and usability.

If you use this data or code, please provide proper credit to the Wikimedia Foundation as the source of the data and the example notebook as a source of the software.
