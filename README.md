# Telecom-Dataset-analysis-and-ML-model


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Telecom Customer Churn Analysis</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 40px;
            background-color: #f5f7fa;
            color: #333;
        }
        h1, h2, h3 {
            color: #2c3e50;
        }
        .container {
            max-width: 900px;
            margin: auto;
            background: #fff;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        .badge {
            display: inline-block;
            padding: 5px 10px;
            background: #3498db;
            color: #fff;
            border-radius: 5px;
            margin: 5px 5px 5px 0;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 15px;
        }
        table, th, td {
            border: 1px solid #ddd;
        }
        th, td {
            padding: 10px;
            text-align: center;
        }
        th {
            background-color: #3498db;
            color: white;
        }
        ul {
            line-height: 1.6;
        }
        .highlight {
            color: green;
            font-weight: bold;
        }
    </style>
</head>
<body>

<div class="container">

    <h1>📊 Telecom Customer Churn Analysis</h1>

    <h2>📌 Project Overview</h2>
    <p>
        This project analyzes telecom customer data to identify churn patterns and predict customer behavior 
        using machine learning techniques.
    </p>

    <h2>📂 Dataset Information</h2>
    <ul>
        <li><b>Total Records:</b> 7,043</li>
        <li><b>Total Features:</b> 21</li>
        <li><b>Null Values:</b> 0</li>
        <li><b>Duplicates:</b> 0</li>
    </ul>

    <h3>🔧 Data Preprocessing</h3>
    <ul>
        <li>Converted <b>total_charges</b> → float</li>
        <li>Converted <b>senior_citizen</b> → Yes/No</li>
        <li>Renamed columns to snake_case</li>
    </ul>

    <h2>📊 Exploratory Data Analysis</h2>
    <ul>
        <li>26.5% customers churned</li>
        <li>Month-to-month contracts → highest churn</li>
        <li>Electronic check → high churn rate</li>
        <li>Low tenure + no add-ons → high risk</li>
    </ul>

    <h2>🤖 Machine Learning Models</h2>

    <table>
        <tr>
            <th>Model</th>
            <th>Accuracy</th>
            <th>Precision</th>
            <th>Recall</th>
            <th>F1 Score</th>
        </tr>
        <tr>
            <td>Logistic Regression</td>
            <td>80.6%</td>
            <td>0.66</td>
            <td>0.56</td>
            <td>0.60</td>
        </tr>
        <tr>
            <td>Decision Tree</td>
            <td>72.6%</td>
            <td>0.63</td>
            <td>0.54</td>
            <td>0.58</td>
        </tr>
        <tr>
            <td>Random Forest</td>
            <td>80.6%</td>
            <td>0.68</td>
            <td>0.51</td>
            <td>0.58</td>
        </tr>
        <tr>
            <td><b>Gradient Boosting 🏆</b></td>
            <td class="highlight">85.1%</td>
            <td>0.77</td>
            <td>0.65</td>
            <td class="highlight">0.70</td>
        </tr>
    </table>

    <h2>🏆 Best Model</h2>
    <p>
        <b>Gradient Boosting</b> achieved the best performance with:
    </p>
    <ul>
        <li>Accuracy: 85.1%</li>
        <li>F1 Score: 0.70</li>
        <li>AUC: 0.914</li>
    </ul>

    <h2>📌 Key Business Insights</h2>
    <ul>
        <li>Short tenure customers churn more</li>
        <li>Contract type impacts retention</li>
        <li>Payment method affects churn</li>
    </ul>

    <h2>🛠️ Tech Stack</h2>
    <div>
        <span class="badge">Python</span>
        <span class="badge">Pandas</span>
        <span class="badge">NumPy</span>
        <span class="badge">Scikit-learn</span>
        <span class="badge">XGBoost</span>
    </div>

    <h2>🚀 How to Run</h2>
    <pre>
git clone https://github.com/your-username/telecom-churn-analysis.git
pip install -r requirements.txt
jupyter notebook
    </pre>

    <h2>👨‍💻 Author</h2>
    <p><b>Prabhat Prajapati</b></p>

</div>

</body>
</html>
