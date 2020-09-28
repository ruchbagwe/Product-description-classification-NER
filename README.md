# Product-description-classification-NER
Product classification by performing entity recognition from product description using NER
## Dataset
Laptops data scrapped from the eBay website using Beautifulsoup. Entities are the laptop description (Product Brand, Product Model, Hard disk type/size, display type, etc.) available on the eBay site.

## Data cleaning and preprocessing 
Data is cleaned and arrange in the CSV file. The laptop’s model names are then standardized by replacing the model name by the standard version of the laptop.

## Tokenizing
Data is tokenized by jumbling the entities and by creating the Product Name as content. Then entities are annotated with start and endpoints and stored in JSON format

## Training model
To train the NER model. First blank Spacy model is created, and the entities are updated with the above entities.
Then the NER model is trained with dropout 0.2 and 30 iterations.
