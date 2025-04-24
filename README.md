# Carcinogens within Cosmetics 




## Table of Contents
* [Tableau Dashboard](#Tableau-dashboard)
* [Motivation](#motivation)
* [Questions](#questions)
* [Normalizing the Data](#normaling-the-data)
* [Problems and Hurdles](#problems-and-hurdles)
* [Technologies Used](#technologies-used)
* [Sources](#sources)
* [Conclusion](#conclusion)

## Tableau Dashboard
Link:

## Motivation:
As someone who regularly uses cosmetics to improve my mental health.I wanted to better undertand the potential health risks associated with common cosmetic ingredients. This dashboard was driven by a desire to identify harmful chemicals found in everyday cosmetic products and to make more informed choices as a consumer. By uncovering which ingredients are potentially dangerous and which companies use them, I hope to raise awareness of carcinogens found in cosmetics as well as pointing out the lack of research of chemicals within cosmetic products.


## Questions:
1) Which chemicals are the most common in cosmetic products? titanium
2) Is the most used chemical a carcinogen?
3) Can cosmetic consumers easily link cosmetic ingredients to carcinogens?
4) Are cosmetic companies trying to provide consumers with safe products?
5) Is there enough research being done on the chemicals used in cosmetics?



## Normalizing the Data
To conduct this analysis, I used two seperate datasets: the IARC Human Carcinogen Monograph and the California Safe Cosmetic Products Program(CSCP) database. The IARC dataset provided information on carcinogens including classification groups, publication dates, and usage volumes. The CSCP dataset included product names, associated companies, associated brands, as well as the year the product year information. By combining these two sources, I was able to associate each product with its carcinogen classification, enabling a more comprehensive look at chemical safety. 

## Problems and Hurdles
One of the major challenges was data availability, since the fda does not require cosmetic ingredients to be pre-approved, and there's no centralized registy of products and their chemical contents.To overcome this, I sourced data from states that maintain public databases-specifically, the CSCP. The biggest hurdle was cleaning and merging the dataset made it difficult to match entries. To solve this, I used the RapidFuzzy library for fuzzy matching, allowing me to standardize chemical names and align them with the IARC dataset for accurate classificatio. 

## Technologies Used
1) Python / Pandas - for exploration, normalizing and aggregation of the dataset
2) Tableau - for creating introduction and interactive dashboard 
3) Git - for version control

## Data Sources
To answer the above questions I used the following sources to collect datasets for my analysis

1) International Agency for Research-IARC monograph on the Identification of Carcinogenic Hazards to Humans-.
https://monographs.iarc.who.int/list-of-classifications/

2) California Department of Puble Health-California Safe Cosmetics Program (CSCP) Product Database.
https://cscpsearch.cdph.ca.gov/search/publicsearch

3) US Food & Drug Administration (general information)- Information of reporting cosmetic product information
https://www.fda.gov/cosmetics/cosmetic-products-ingredients/cosmetic-ingredients


## Conclusion
The data visualization highlighs critical insights into thecosmetic industry's us of chemicals with a specific focus on carcinogenic risks.The analysis shows that while titanium is the most frequently used chemical, it is not classified as a carcinogen. Additionally, cosmetic consumers face difficulty linking ingredients to carcinogens, indicating a lock of transparaency in labeling or public awareness. Despite these challenges, the data suggests that many cosmetic companies are making efforts to provide safer products. However, there remains a significant gap in research on the chemicals used in cosmetics, underscoring the need for continued investigation and improved regulatory oversight to ensure consumer safety. 
