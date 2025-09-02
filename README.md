# Player Performance Clustering Analysis

This project uses unsupervised machine learning, specifically K-Means clustering, to analyze Fantasy Premier League (FPL) player data and identify distinct player archetypes based on their statistical performance.

### Project Goal

The primary goal of this analysis is to group football players into meaningful clusters, providing insights into different player roles beyond their official positions. By analyzing the key features that define each cluster, we can understand the underlying performance profiles of players and their contributions to a fantasy football team.

### Methodology

The analysis follows these key steps:
1.  **Data Loading and Preprocessing**: The project loads player data from `fpl_data.csv`. The data is then preprocessed to handle missing values and scale numerical features, preparing it for clustering.
2.  **Clustering**: The K-Means algorithm is applied to the processed data to partition players into a specified number of clusters. The optimal number of clusters is determined to ensure a meaningful and robust grouping.
3.  **Cluster Analysis**: The final clusters are analyzed by comparing the average feature values of each cluster against the global mean. This reveals the most positively different features for each group, which are then used to interpret and name the player archetypes.

### Results

The analysis identified three distinct player clusters, each representing a unique archetype:

* **Cluster 0: The Attacking Dynamo**
    * **Description:** Players defined by offensive metrics like goals, assists, threat, and creativity.
    * **Player Type:** Forwards and attacking midfielders.

* **Cluster 1: The Workhorse Defender**
    * **Description:** Players with high total points and minutes, but also a mixed defensive record (high clean sheets and goals conceded).
    * **Player Type:** Starting defenders and goalkeepers.

* **Cluster 2: The Influential Defender**
    * **Description:** Players with high defensive influence, in addition to consistent playing time and defensive stats.
    * **Player Type:** Central defenders and full-backs.

### Files in this Repository

* `fpl_data.csv`: The dataset containing player statistics used for the analysis.
* `sports_clustering_analysis.ipynb`: A Jupyter Notebook containing the full code for the data preprocessing, clustering, and analysis.

2.  
3.  **Run the Notebook:** Open the `sports_clustering_analysis.ipynb` file in a Jupyter Notebook environment to view and execute the analysis code.
