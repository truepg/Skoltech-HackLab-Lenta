# The hack by LENTA and Skoltech Hacklab.

## Task
Customer clustering based on transactions.

## Pipeline
1. Build the customer buckets as list of favorite products in each category (lowest level of hierarchy).
2. Use word2vec to obtain products embeddings, where "texts" are the customer buckets and "words" are the products.
3. Use TF-IDF weighting of products embeddings to get customer (bucket) embeddings.
4. Use agglomerative clustering with cosine measure over customer embeddings to obtain customer clusters.
