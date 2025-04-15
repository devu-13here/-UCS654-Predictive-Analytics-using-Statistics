
   <h1>Clustering Evaluation with Preprocessing Techniques</h1>

   <div class="section">
        <h2>📄 Description</h2>
        <p>
            This project performs clustering on the <b>Iris dataset</b> using three algorithms:
            <ul>
                <li><b>KMeans</b></li>
                <li><b>Hierarchical (Agglomerative)</b></li>
                <li><b>MeanShift</b></li>
            </ul>
            Various preprocessing techniques like normalization, transformation, and PCA are applied to the dataset before clustering.
        </p>
    </div>

  <div class="section">
        <h2>⚙️ Preprocessing Techniques</h2>
        <ul>
            <li><b>No Data Processing</b>: Raw data is used</li>
            <li><b>Normalization</b>: Scales data between 0 and 1</li>
            <li><b>Transform</b>: Applies log1p transformation</li>
            <li><b>PCA</b>: Reduces data to 2D using Principal Component Analysis</li>
            <li><b>Transform + Normalize</b></li>
            <li><b>Transform + Normalize + PCA</b></li>
        </ul>
    </div>

   <div class="section">
        <h2>📊 Evaluation Metrics</h2>
        <p>For each clustering result, the following evaluation metrics are computed:</p>
        <ul>
            <li><code>Silhouette Score</code>: Measures cohesion vs separation</li>
            <li><code>Calinski-Harabasz Score</code>: Ratio of dispersion between and within clusters</li>
            <li><code>Davies-Bouldin Score</code>: Lower score is better; indicates cluster separation</li>
        </ul>
    </div>

   <div class="section">
        <h2>🧪 Cluster Counts</h2>
        <p>For <b>KMeans</b> and <b>Hierarchical</b>, clustering is performed with <b>3</b>, <b>4</b>, and <b>5</b> clusters.</p>
        <p><b>MeanShift</b> clustering auto-determines the number of clusters based on data distribution.</p>
    </div>

  <div class="section">
        <h2>📝 Output</h2>
        <ul>
            <li>Clustering results are printed for each algorithm and preprocessing method.</li>
            <li>Results are also saved as:
                <ul>
                    <li><code>kmeans_results.csv</code></li>
                    <li><code>hierarchical_results.csv</code></li>
                    <li><code>meanshift_results.csv</code></li>
                </ul>
            </li>
        </ul>
    </div>

  <div class="section">
        <h2>▶️ How to Run</h2>
        <ol>
            <li>Install requirements:
                <pre><code>pip install numpy pandas scikit-learn</code></pre>
            </li>
            <li>Run the script:
                <pre><code>python clustering_analysis.py</code></pre>
            </li>
        </ol>
    </div>

   <div class="section">
        <h2>📁 Files</h2>
        <ul>
            <li><code>clustering_analysis.py</code>: Main Python script</li>
            <li><code>kmeans_results.csv</code>: Output from KMeans</li>
            <li><code>hierarchical_results.csv</code>: Output from Hierarchical</li>
            <li><code>meanshift_results.csv</code>: Output from MeanShift</li>
        </ul>
    </div>

   <div class="section">
        <h2>💡 Notes</h2>
        <p>If a clustering model returns only one cluster, evaluation metrics will show <code>None</code> due to undefined calculations.</p>
    </div>
</body>
</html>

![meanshift_results](https://github.com/user-attachments/assets/930eac6d-0d12-48a5-b3b7-0dd89391000f)

![kmeans_results](https://github.com/user-attachments/assets/8fd4cf40-a0e0-4084-a417-3397495bbb4c)

![hierarchical_results](https://github.com/user-attachments/assets/ac0bc470-5c19-4132-9628-bfa2630108aa)
