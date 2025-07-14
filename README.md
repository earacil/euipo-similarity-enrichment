# EUIPO Similarity Enrichment DEMO

This project contains two main Python notebooks. 
* `taxo_tree_builder.ipynb` generates the taxonomies from a JSON file named `taxo_jsontree_20250627.json` stored in `/data`. 
* `new_similarity_relationships.ipynb` supports two tasks: one that finds taxonomy nodes similar to each other without an existing **HAS_SIMILARITY** relationship (an example output for nodes selected via PageRank is in `/data/result1.txt`), and another that, given a question, identifies the most similar class and retrieves all its taxonomy data. 

### Data

The `/data` folder also holds the model `neo4j_importer_model_2025-07-09.json` for importing into Aura the `ST_Dataset_main_fields_similarity_int.csv`.

### Dependencies

- pip install dotenv pypdf openai utils rdflib neo4j langchain langchain-community tiktoken