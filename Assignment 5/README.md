![image](https://github.com/user-attachments/assets/32cbae4c-16a9-45df-a5fe-744295323663)

  <h1>Optimized SVM on UCI Multi-Class Dataset</h1>

  <h2>📌 Objective</h2>
  <p>To implement and optimize a Support Vector Machine (SVM) classifier on a multi-class dataset from the UCI Machine Learning Repository using parameter tuning and convergence analysis.</p>

  <h2>📂 Dataset</h2>
  <p>
    Dataset: <strong>Letter Recognition</strong><br>
    Source: <a href="https://archive.ics.uci.edu/ml/datasets/letter+recognition" target="_blank">UCI Repository</a><br>
    Size: 20,000+ rows<br>
    Classes: 26 (A to Z)
  </p>

  <h2>🧪 Task Breakdown</h2>
  <ul>
    <li>Split dataset into 10 different random samples (each with 70% training and 30% testing).</li>
    <li>Run SVM optimization for 100 iterations on each sample.</li>
    <li>Test different SVM parameters: <strong>Kernel</strong>, <strong>Nu</strong>, <strong>Epsilon</strong>.</li>
    <li>Record the best accuracy and parameters per sample.</li>
    <li>Plot convergence graph of the most accurate sample.</li>
    <li>Perform basic data analysis (shape, nulls, class distribution).</li>
  </ul>

  <h2>🔍 Optimization Strategy</h2>
  <p>
    Used <code>NuSVC</code> from <strong>scikit-learn</strong> with random sampling of parameters:<br>
    Kernels: linear, rbf, poly, sigmoid<br>
    Nu: range from 0.01 to 1<br>
    Epsilon: range from 0.01 to 1 (stored but not used directly in NuSVC)<br>
  </p>

  <h2>📈 Results</h2>
  <p>Saved in <code>svm_optimization_results.csv</code></p>

  <h3>Sample Table Format</h3>
  <table>
    <tr>
      <th>Sample #</th>
      <th>Best Accuracy (%)</th>
      <th>Kernel</th>
      <th>Nu</th>
      <th>Epsilon</th>
    </tr>
    <tr>
      <td>S1</td>
      <td>94.2</td>
      <td>rbf</td>
      <td>0.5</td>
      <td>0.1</td>
    </tr>
    <!-- More rows populated by script -->
  </table>

  <h2>📊 Convergence Graph</h2>
  <p>Shows accuracy improvements over 100 iterations for the best-performing sample.</p>
  <img src="convergence_plot_sample.png" alt="Convergence Plot" width="600">

  <h2>📊 Data Analysis</h2>
  <ul>
    <li><strong>Dataset shape:</strong> 20000 rows, 16 features</li>
    <li><strong>Missing values:</strong> None</li>
    <li><strong>Class distribution:</strong> Evenly distributed A-Z</li>
  </ul>

  <h2>💾 Repository Contents</h2>
  <ul>
    <li><code>svm_optimization.py</code> — full source code</li>
    <li><code>svm_optimization_results.csv</code> — accuracy and parameters for 10 samples</li>
    <li><code>convergence_plot_sample.png</code> — graph of accuracy over iterations</li>
    <li><code>README.html</code> — this file</li>
  </ul>

  <h2>🚀 How to Run</h2>
  <div class="code-block">
    pip install pandas numpy scikit-learn matplotlib seaborn<br>
    python svm_optimization.py
  </div>

  <h2>📬 Contact</h2>
  <p>For questions, feel free to open an issue or contact via GitHub.</p>

</body>
</html>

