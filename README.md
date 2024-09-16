# Distributed Database Management - Spark
1.	Data Preprocessing:

•	Normalized numerical variables and applied one-hot encoding to categorical variables.
This ensures fair comparison between features and prevents misinterpretation of categorical data. It's crucial for accurate modeling and analysis, especially when dealing with diverse demographic data.
3.	Dimensionality Reduction:
•	Used SVD to project feature vectors onto 2D space.
This revealed the principal components with the largest singular values, capturing the direction of maximum variance. It helped identify three main clusters in the data, providing initial insights into household groupings.
4.	Clustering:
•	Applied K-means algorithm with 8 clusters.
This grouping allows for more targeted analysis of household characteristics and viewing habits. The choice of 8 clusters was an initial approach to segment the data.
5.	Visualization of Clusters:
•	Used PCA for 2D reduction and created a color-coded scatter plot.
This visualization revealed varying levels of cluster overlap. I noted that reducing to 6 clusters might provide more distinct groupings, demonstrating my ability to critically evaluate and adjust methodologies.
6.	Viewing Analysis:
•	Calculated 'diff rank' for stations in each cluster/subset.
Explanation: This metric reveals how viewing preferences in each cluster differ from the general population. I found that the 'diff rank' values were generally low (below 0.8), indicating no strong preferences for particular stations across clusters.
7.	Streaming Analysis:
•	Used Spark Streaming to process viewing data from Kafka.
This demonstrates handling real-time data, crucial for keeping recommendations current. I observed high similarity in top-10 stations across triggers for each cluster, suggesting consistent viewing patterns within clusters over time.
8.	Key Insights:
•	Cluster consistency: The similarity in results across different subset types within clusters indicates stable viewing preferences as data volume increases.
•	Decreasing 'diff rank': I noticed that 'diff rank' decreased across triggers, suggesting that cluster-specific viewing habits were converging towards general population trends over time.
•	Visualization approach: I created a multi-panel visualization for efficient data analysis, showcasing my ability to present complex data clearly.
I recognized that the chosen number of clusters and dimensionality reduction didn't provide clear insights into specific viewing preferences. This demonstrates my ability to critically assess the effectiveness of analytical approaches.
By explaining these aspects, I show not only technical proficiency in data preprocessing, machine learning, and streaming analytics, but also the ability to derive meaningful insights, critically evaluate methodologies, and suggest improvements. This balanced approach of technical skills and analytical thinking is valuable in data science roles

