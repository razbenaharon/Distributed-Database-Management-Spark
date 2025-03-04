🚀 Distributed Database Management - Spark
This project focuses on data preprocessing, dimensionality reduction, clustering, and real-time streaming analysis using Apache Spark. The goal is to segment households based on viewing habits and derive meaningful insights from large-scale demographic data.

📌 Key Components
1️⃣ Data Preprocessing
✅ Normalized numerical variables and applied one-hot encoding to categorical variables.
🔹 Ensures fair comparison between features and prevents misinterpretation of categorical data.
🔹 Crucial for accurate modeling and analysis, especially with diverse demographic datasets.

2️⃣ Dimensionality Reduction
✅ Used Singular Value Decomposition (SVD) to project feature vectors onto a 2D space.
🔹 Revealed principal components with the largest singular values, capturing maximum variance.
🔹 Helped identify three main clusters, providing initial insights into household groupings.

3️⃣ Clustering
✅ Applied K-means clustering with 8 clusters.
🔹 Allowed for targeted analysis of household characteristics and viewing habits.
🔹 The choice of 8 clusters was an initial approach to segment the data, with further evaluation planned.

4️⃣ Visualization of Clusters
✅ Used PCA for 2D reduction and created a color-coded scatter plot.
🔹 Revealed varying levels of cluster overlap, indicating possible cluster refinements.
🔹 Identified that reducing to 6 clusters might provide more distinct groupings, showcasing an analytical approach to methodology improvement.

5️⃣ Viewing Analysis
✅ Calculated 'diff rank' for stations in each cluster/subset.
🔹 Purpose: Measures how viewing preferences in each cluster differ from the general population.
🔹 Findings:

'Diff rank' values were generally low (below 0.8), indicating no strong preferences for particular stations across clusters.
Suggests that household viewing patterns may be more uniform than initially expected.
6️⃣ Streaming Analysis
✅ Used Spark Streaming to process real-time viewing data from Kafka.
🔹 Demonstrates real-time data processing, crucial for keeping recommendations current.
🔹 Findings:

High similarity in Top-10 stations across different time triggers.
Suggests consistent viewing patterns within clusters over time.
📊 Key Insights & Observations
🔹 Cluster Consistency:

High similarity in results across different subset types indicates stable viewing preferences as data volume increases.
🔹 Decreasing 'Diff Rank' Over Time:

Observed a gradual decline in diff rank across triggers.
Suggests that cluster-specific viewing habits were converging toward general population trends.
🔹 Visualization Strategy:

Implemented multi-panel visualizations for efficient data analysis.
Demonstrates the ability to present complex data clearly and meaningfully.
🔍 Reflection & Next Steps
❌ Identified that the chosen number of clusters & dimensionality reduction method may not fully capture specific viewing preferences.
✅ Demonstrates strong analytical thinking—critically assessing the effectiveness of models and suggesting improvements.
✅ Showcases technical proficiency in:

Data Preprocessing
Machine Learning for Clustering
Streaming Analytics with Spark
Effective Data Visualization & Insights Extraction
This balance between technical execution and analytical evaluation is essential for data science and engineering roles. 🚀

⚡ Tech Stack Used
Apache Spark (PySpark)
Kafka (Streaming Data)
Pandas & NumPy (Preprocessing)
Matplotlib & Seaborn (Visualization)
K-Means, SVD, PCA (Machine Learning)
