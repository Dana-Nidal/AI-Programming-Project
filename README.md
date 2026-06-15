# AI Programming Final Project: COVID-19 Clustering Analysis in Indonesia

**Author:** Dana Nidal 
  ---

## Project Overview
This project focuses on grouping and analyzing the severity of the COVID-19 pandemic across different provinces in Indonesia using unsupervised machine learning. By utilizing **K-Means Clustering**, the model categorizes provinces into separate clusters based on three primary epidemiological metrics:
* **Confirmed Cases**
* **Recovered Cases**
* **Deaths**

The results of this model are compared directly against findings from an existing research paper to assess accuracy, cluster characteristics, and geographical distribution behavior.

## Dataset Description
The model reads data containing COVID-19 statistics per Indonesian province with the following structure:
* `Province`: Name of the specific region (used as a label/identifier).
* `Confirmed`: Total confirmed positive cases.
* `Recovered`: Total patients recovered.
* `Deaths`: Total reported fatalities.

## Libraries & Tools Used
The script is written in Python 3 within a Jupyter Notebook environment, leveraging the following essential data science libraries:
* **Pandas & NumPy**: For data manipulation, filtering features from labels, and descriptive statistical analysis.
* **Matplotlib**: For generating exploratory visualizations (such as case distribution bar plots).
* **Scikit-learn (Sklearn)**:
  * `StandardScaler`: For normalizing feature scales.
  * `KMeans`: For building and training the clustering model.
  * `silhouette_score`: For evaluating cluster coherence.

## Key Findings & Model Comparison
* **High Similarity:** The trained K-Means model yielded results highly consistent with the benchmark research paper.
* **Cluster Numbering Difference:** While the research paper designated its clusters as 1, 2, and 3, this model uses Python's 0-indexed layout, categorizing them into clusters 0, 1, and 2.
* **Banten Province Variance:** The only major difference observed was the grouping of the **Banten** province. The model categorized it into Cluster 2, whereas the original paper placed it into Cluster 1. All other provincial clusters remain identical to the paper.
