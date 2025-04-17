
![sampling_accuracy_table](https://github.com/user-attachments/assets/347245ed-d8c1-4e20-81c8-2a6f7c0c8cc3)

  <h1>Credit Card Fraud Detection with Sampling Techniques</h1>

  <h2>📌 Objective</h2>
    <p>
        This project aims to evaluate the performance of five machine learning models on a credit card fraud detection dataset using different sampling techniques to handle class imbalance.
    </p>

   <h2>📁 Dataset</h2>
    <p>
        The dataset used is <code>Creditcard_data.csv</code>, which contains features extracted from credit card transactions along with a binary target variable <code>Class</code>, indicating fraud (1) or not (0).
    </p>

   <h2>🔧 Preprocessing</h2>
    <ul>
        <li>Missing values checked (none found).</li>
        <li>Data scaled using <code>StandardScaler</code>.</li>
        <li>Class imbalance resolved using <code>SMOTE</code>.</li>
        <li>Five samples created (each ~400 rows) using statistical sampling formula.</li>
    </ul>

  <h2>🧠 Models Used</h2>
    <ul>
        <li><strong>M1:</strong> Logistic Regression</li>
        <li><strong>M2:</strong> Decision Tree</li>
        <li><strong>M3:</strong> Random Forest</li>
        <li><strong>M4:</strong> Naive Bayes</li>
        <li><strong>M5:</strong> Gradient Boosting</li>
    </ul>

   <h2>🧪 Sampling Techniques</h2>
    <ul>
        <li><strong>Sampling1:</strong> Random Under Sampling</li>
        <li><strong>Sampling2:</strong> Random Over Sampling</li>
        <li><strong>Sampling3:</strong> SMOTE</li>
        <li><strong>Sampling4:</strong> NearMiss</li>
        <li><strong>Sampling5:</strong> SMOTETomek</li>
    </ul>

   <h2>📊 Accuracy Matrix</h2>
    <p>
        A 5x5 accuracy matrix was computed where each model was evaluated using each sampling technique.
    </p>

   <h2>🏆 Best Technique per Model</h2>
    <p>
        The sampling method achieving the highest accuracy for each model was identified.
    </p>

   <h2>🚀 Output</h2>
    <ul>
        <li>Accuracy Matrix printed in console</li>
        <li>Best sampling strategy per model displayed</li>
    </ul>

   <h2>🗃️ Project Structure</h2>
    <pre>
    ├── Creditcard_data.csv
    ├── Assignment2_102216050.ipynb
    ├── sampling_accuracy_table.png
    └── README.html
    </pre>

   <h2>🔗 Submission</h2>
    <p>
        Push all files to GitHub, including this <code>README.html</code>, code notebook, dataset summary, accuracy matrix PNG, and sampling comparison discussion.
    </p>

</body>
</html>

