# MoviePlotClustering

UWB CSS 586 Deep Learning Research Project: Clustering Movie Plot Summary Embeddings

## ACM Conference Paper (Draft)

[Movie Genre Discovery: Clustering Plot Summary Embeddings](https://drive.google.com/file/d/1Ftk1xabZ--9k4IpOYQ3scjdqx3IA2u3c/view?usp=sharing)

## About

This project aims to enhance movie genre categorization by employing natural language processing techniques. We analyzed movie plot summaries using various combinations of embedding architectures (Word2Vec, SBERT, Longformer) and clustering methods (K-Means and Spectral Clustering). The SBERT and Spectral Clustering combination yielded the most meaningful movie clusters, providing a promising foundation for fine-grained genre discovery. These findings have potential applications in movie recommendation systems or content discovery platforms. Future work may further improve the quality of clusters and capture nuanced movie themes.

Notebooks already contain results from existing runs. Open in github or VSCode to view results. To run/modify notebooks, follow the quickstart guide below.

## Notebook Filename Convention

`[Embedding Algorithm]-[Clustering Technique]-[Dataset]-[# of Movies Used]-[# of Clusters]-[EXTRA]`

## Datasets

[CMU Corpus for extended synopsis](https://www.cs.cmu.edu/~ark/personas/)

[TMDB Corpus for plot summaries](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata?datasetId=138)

## Quickstart

The notebooks are executable on Kaggle. Both datasets must be imported to Kaggle before runtime. To run a notebook on Kaggle:

1. Open a new notebook
2. Navigate to File -> Import Notebook, and select the notebook you want to open
3. On the right-hand data pane, click 'Add Data'. Then:
    - Search for `TMDB 5000 Movie Dataset` and add it.
4. Manually upload the modified `CMU Corpus Dataset` from this repo:
    - Click the 'Upload' icon button on the right-hand data pane
    - Enter dataset title `movieplotsummarydata`
    - Browse for `FinalMovieData.tsv` (contained in this repo) and click 'Create'
    - Note: After importing subsequent notebooks, click add data and add `movieplotsummarydata`, since it has already been uploaded.
5. Run all cells as desired

## Accelerated Resources

To run the Longformer notebooks (pre-fixed with `Longformer`), you must enable TPU-accelerated hardware on kaggle. On the notebook page, click the 3 vertical dots in the upper right-hand corner and select `TPU VM v3-8` under `Accelerator`. Select `Turn On` if pop-up warning occurs, or click the start button to enable the TPU-accelerated hardware session. You can now run the notebook
