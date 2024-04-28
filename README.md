# Detecting Duplicate Product Titles in Foodpanda's Product Catalog 

## Approach:

Our strategy for identifying duplicate product titles involves using a similarity algorithm called cosine similarity. Cosine similarity is a measure of similarity between two non-zero vectors in an inner product space that measures the cosine of the angle between them. In the context of natural language processing (NLP) and text analysis, cosine similarity is often used to quantify the similarity between two documents or pieces of text represented as vectors in a high-dimensional space.

### 1.  Detecting Duplicate Product Titles

This code performs text similarity analysis on product names extracted from an Excel file ('catalog.xlsx'). After reading the Excel file and extracting relevant columns ('product_name_english' and 'encrypt_master_code'), it employs TF-IDF (Term Frequency-Inverse Document Frequency) vectorization to convert the product names into numerical representations. Then, it calculates the cosine similarity matrix to measure the similarity between all pairs of product names. Next, it identifies duplicate product titles and stores their indices along with corresponding master codes in a dictionary. Finally, it creates an output DataFrame containing pairs of duplicate product names and their associated master codes, saving the result to an Excel file named 'duplicate_products_with_master_codes.xlsx'.


## Results:

This code processes product data from an Excel file, identifying duplicate product titles and their associated master codes. The resulting output is stored in an Excel file with three columns: 

1. Duplicates: This column contains comma-separated lists of duplicate product titles.
2. Master Codes: Each entry in this column represents the master codes corresponding to the similar products. The master codes are enclosed in curly braces and separated by commas.
3. Count: This column indicates the total count of duplicates for each set of similar products.




