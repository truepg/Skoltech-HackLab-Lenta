# The hack by LENTA and Skoltech Hacklab.

## Task
Customer clustering.

## Pipeline
1. Build customer buckets (list of favourite products in each category (lowest level of hierarchy)
2. Use word2vec to obtain products embeddings (texts = customer buckets, words = products)
3. Use tf-idf weighting of products embeddings to get customers (buckets) embeddings
4. Use agglomerative clustering with cosine measure over customer embeddings to obtain customer clusters
