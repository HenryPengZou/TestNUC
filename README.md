# TestNUC: Enhancing Test-Time Computing Approaches and Scaling through Neighboring Unlabeled Data Consistency


<!-- ![Task](code/images/scaling.jpg) -->


This repository contains the implementation of the paper:
> **TestNUC: Enhancing Test-Time Computing Approaches and Scaling through Neighboring Unlabeled Data Consistency** 
> [[Paper]](https://aclanthology.org/2025.acl-long.1486.pdf) [[ACL Anthology]](https://aclanthology.org/2025.acl-long.1486/) [[arXiv]](https://arxiv.org/abs/2502.19163) <br>
> The 63rd Annual Meeting of the Association for Computational Linguistics, ACL 2025 <br>
> Henry Peng Zou, Zhengyao Gu, Yue Zhou, Yankai Chen, Weizhi Zhang, Liancheng Fang, Yibo Wang, Yangning Li, Kay Liu, Philip S. Yu <br>



## Quick Start


### 1. Obtain Embeddings

You can download pre-extracted embeddings from this [Google Drive Folder](https://drive.google.com/drive/folders/1Y6QhJW9nb3objSHQue0rA3pmT4cvcg2f):

```bash
gdown --folder https://drive.google.com/drive/folders/1Y6QhJW9nb3objSHQue0rA3pmT4cvcg2f -O ./data/
```

You can also choose to extract embeddings by yourself from any embedder on [Huggingface Embedder Leaderboard](https://huggingface.co/spaces/mteb/leaderboard) by following their insturction, e.g., [Qwen Embedder Usage](https://huggingface.co/Qwen/Qwen3-Embedding-8B#usage).



### 2. (Optional) Pseudo Labeling / Obtain Initial LLM Predictions

Extract inital LLM predictions by running `pseudo_labeling.ipynb` in the `scripts_llm` folder.


### 3. Neibhor Retrieval & Collaborative Prediction

Simply run `aggregation_num_unlabeled_data.ipynb` in the `scripts_llm` folder.


Feel free to reach out to me if you want the code early or have any questions. (email: pzou3@uic.edu)


