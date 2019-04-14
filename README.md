# Run-Experiments
---

## General Idea  :

Run Experiments is a Java Class used to automatically run different information retrieval Experiments Automatically based on different input variables.

## Input & Output

### Input Parameters :
* Retrieval Models (BM25 - PL2 and LMD) and ranges of their associated values (b,k,c,mu)

| Retrieval Model | Range Values |
|:---:|:---:|
|BM25|b,k|
|PL2|c|
|LMD|c|

* Indices ( It is preferable to create the index using IndexerApp from https://github.com/lucene4ir/lucene4ir/blob/master/README.md __in order to match token filters with the run experiments__
* Query Files
* Qrel Files
* Token Filters . Token Filters used for creating the index and retrieval experiment should be the same
![Input Explanation](https://user-images.githubusercontent.com/47518534/56099576-a984b580-5f06-11e9-938e-185cdf3798b9.jpg "Input Explanation")

### Output Results :

