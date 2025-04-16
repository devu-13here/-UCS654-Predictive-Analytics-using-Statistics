![image](https://github.com/user-attachments/assets/32cbae4c-16a9-45df-a5fe-744295323663)



  <h1>📊 SVM Optimization on Dry Bean Dataset</h1>

  <h2>📌 Objective</h2>
  <p>
    The goal of this project is to optimize a Support Vector Machine (SVM) classifier for the
    <strong>Dry Bean Dataset</strong> from the UCI Machine Learning Repository using various SVM parameters and analyze the convergence of model performance.
  </p>

  <h2>📂 Dataset Info</h2>
  <ul>
    <li><strong>Name:</strong> Dry Bean Dataset</li>
    <li><strong>Source:</strong> <a href="https://archive.ics.uci.edu/ml/datasets/Dry+Bean+Dataset" target="_blank">UCI ML Repository</a></li>
    <li><strong>Instances:</strong> 13,611</li>
    <li><strong>Features:</strong> 16 numerical</li>
    <li><strong>Classes:</strong> 7 types of beans</li>
  </ul>

  <h2>🧪 Project Steps</h2>
  <ol>
    <li>Loaded and analyzed the Dry Bean dataset.</li>
    <li>Split the dataset into 10 randomized samples (70% train, 30% test).</li>
    <li>Ran 100 iterations of SVM optimization per sample, varying:
      <ul>
        <li>Kernel: linear, rbf, poly, sigmoid</li>
        <li>Nu: 0.01 to 1</li>
        <li>Epsilon: 0.01 to 1 (tracked but not used in NuSVC)</li>
      </ul>
    </li>
    <li>Recorded the best accuracy and parameters for each sample.</li>
    <li>Plotted a convergence graph for the most accurate sample.</li>
    <li>Saved all results to CSV.</li>
  </ol>

  <h2>📈 Sample Result Table Format</h2>
  <table>
    <thead>
      <tr>
        <th>Sample</th>
        <th>Best Accuracy (%)</th>
        <th>Kernel</th>
        <th>Nu</th>
        <th>Epsilon</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>S1</td>
        <td>91.65</td>
        <td>rbf</td>
        <td>0.33</td>
        <td>0.18</td>
      </tr>
      <!-- Remaining rows filled dynamically by the script -->
    </tbody>
  </table>

  <h2>📊 Convergence Graph</h2>
  <p>
    A convergence plot is generated for the best-performing sample, visualizing how the model's accuracy improved over the 100 iterations.
  </p>
  <img src="convergence_plot_sample.png" alt="Convergence Plot" width="600">

  <h2>🔍 Data Summary</h2>
  <ul>
    <li><strong>Shape:</strong> 13,611 rows × 17 columns</li>
    <li><strong>Target column:</strong> Class</li>
    <li><strong>Missing Values:</strong> None</li>
    <li><strong>Class Distribution:</strong> Reasonably balanced across 7 classes</li>
  </ul>

  <h2>📁 Repository Contents</h2>
  <ul>
    <li><code>dry_bean_svm.py</code> — Python code for optimization</li>
    <li><code>Dry_Bean_Dataset.csv</code> — Dataset file</li>
    <li><code>dry_bean_svm_results.csv</code> — Table of results</li>
    <li><code>convergence_plot_sample.png</code> — Accuracy vs. iteration plot</li>
    <li><code>README.html</code> — This documentation</li>
  </ul>

  <h2>🚀 How to Run</h2>
  <pre>
pip install pandas numpy matplotlib seaborn scikit-learn
python dry_bean_svm.py
  </pre>

  <h2>📬 Contact</h2>
  <p>For any questions, feel free to open an issue or reach out via GitHub.</p>

</body>
</html>

![df_results](https://github.com/user-attachments/assets/0c34963b-b34a-4ca3-8004-21edd3869a0d)


