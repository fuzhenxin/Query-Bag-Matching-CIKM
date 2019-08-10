# Query-Bag-Matching-CIKM

This repo contains the composed Quora dataset for the short paper "Query-bag Matching]{Query-bag Matching with Mutual Coverage for Information-seeking Conversations in E-commerce" in CIKM 2019. It also contains the detailed experiments of this paper.

# Composed Quora Dataset
- Coming Soon

# Experiment Setup
## Data
- max sequence length: 20
## hCNN
### Convolution2d for cross-attention matrix 
- Conv1: kernel size 6 ; num output 8 ; stride 1 ; paddding "SAME" ; activation Relu ; 
- Max pooling1: pool size 4,4 ; stride 4 ; padding "SAME"
- Conv2: kernel size 4 ; num output 16 ; stride 3 ; paddding "SAME" ; activation Relu ; 
- Max pooling2: pool size 2,2 ; stride 2 ; padding "SAME"
### Convolution1d for query and question
- filters 100 ; kernel size 2/3/4 ; max pooling pool size 20-kernel_size + 1 ; max pooling stride 1
