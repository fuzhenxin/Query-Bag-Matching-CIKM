# Query-Bag-Matching-CIKM

This repo contains the composed Quora dataset for the short paper "Query-bag Matching]{Query-bag Matching with Mutual Coverage for Information-seeking Conversations in E-commerce" in CIKM 2019. It also contains the detailed experiments of this paper.

# An Example of Alime
- An example of the query-bag pair and the corresponding answer.
- User query:
- 怎么电话小二? (How to call you?) 
- Bag (Pre-defined questions):
- 怎么联系你们? (How to contact you?) 
- 客服热线是多少? (What's the hotline?) 
- Answer: 
- 电话是123456 (The phone number is 123456.) 



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
