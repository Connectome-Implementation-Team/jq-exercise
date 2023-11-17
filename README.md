# JQ Exercises
Beer&Chips, 21.11.2013

Helpful resources:
- https://jqlang.github.io/jq/manual/
- https://jqlang.github.io/jq/
- https://formulae.brew.sh/formula/jq
- https://jqplay.org/

## Combine the Answers of Several REST API requests into one Collection

[Search](https://docs.openalex.org/api-entities/works/search-works) some publications using the OpenAlex Rest API.
Use the [paging](https://docs.openalex.org/how-to-use-the-api/get-lists-of-entities/paging) mechanism to fetch several pages of results and store them in separate JSON files.
Now use `jq` to combine these single files into **one** collection of publications.
From the resulting collection make a summary of all publications (title, DOI etc.)

Hint: It is like drinking a milk shake making quite some noise.

## Generate a CSV Report From a REST API's JSON response (credits: Marcel)

Given a [news feed API call](https://feed-prod.unitycms.io/2/newest?count=50), transform the JSON response to a tabular structure and include only articles.
Each article should be described by its title, abstract, and URL.
The table's first row should indicate the column names.

Hint: The required format is quite common in the Excel world.

## Get Selected Properties from a Wikidata Entity

Given a [Wikidata entity](https://www.wikidata.org/w/api.php?action=wbgetentities&ids=Q78&format=json) representing a city, get its geolocation and/or other properties from JSON.
Feel free to choose another entity from Wikidata :-)

Hint: Wikidata properties are documented [here](https://www.wikidata.org/wiki/Wikidata:Database_reports/List_of_properties/all).

