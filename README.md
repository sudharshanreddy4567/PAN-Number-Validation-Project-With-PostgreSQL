<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>PAN Validation Project - README</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            margin: 40px;
            background-color: #f9f9f9;
            color: #333;
            line-height: 1.6;
        }

        h1, h2, h3 {
            color: #2c3e50;
        }

        .logo {
            width: 100px;
            height: auto;
        }

        .header {
            display: flex;
            align-items: center;
            gap: 20px;
            margin-bottom: 30px;
        }

        code {
            background-color: #f4f4f4;
            padding: 2px 6px;
            border-radius: 4px;
            color: #c0392b;
        }

        ul {
            padding-left: 20px;
        }

        .section {
            margin-bottom: 40px;
        }
    </style>
</head>
<body>

    <div class="header">
        <img src="https://upload.wikimedia.org/wikipedia/commons/2/28/Income_Tax_India_Logo.png" alt="PAN Logo" class="logo">
        <h1>PAN Validation Project</h1>
    </div>

    <div class="section">
        <h2>📌 Objective</h2>
        <p>
            This project involves cleaning and validating a dataset containing the Permanent Account Numbers (PAN) of Indian nationals.
            The goal is to ensure each PAN adheres to the official format and is correctly categorized as either <strong>Valid</strong> or <strong>Invalid</strong>.
        </p>
    </div>

    <div class="section">
        <h2>🧹 Data Cleaning and Preprocessing</h2>
        <ul>
            <li><strong>Handle missing data</strong>: Remove rows with missing or incomplete PAN numbers.</li>
            <li><strong>Check for duplicates</strong>: Remove duplicate PAN numbers.</li>
            <li><strong>Trim spaces</strong>: Remove any leading/trailing whitespaces in PAN numbers.</li>
            <li><strong>Standardize letter case</strong>: Convert all PAN numbers to uppercase.</li>
        </ul>
    </div>

    <div class="section">
        <h2>🔍 PAN Format Validation Rules</h2>
        <p>A valid PAN number must meet the following criteria:</p>
        <ul>
            <li>Exactly 10 characters in total.</li>
            <li><strong>First 5 characters</strong>: Alphabetic (A-Z)
                <ul>
                    <li>Adjacent letters cannot be the same (e.g., <code>AABCD</code> is invalid).</li>
                    <li>Cannot be a sequential series (e.g., <code>ABCDE</code> is invalid).</li>
                </ul>
            </li>
            <li><strong>Next 4 characters</strong>: Digits (0-9)
                <ul>
                    <li>Adjacent digits cannot be the same (e.g., <code>1123</code> is invalid).</li>
                    <li>Cannot be a sequential series (e.g., <code>1234</code> is invalid).</li>
                </ul>
            </li>
            <li><strong>Last character</strong>: Alphabetic (A-Z)</li>
        </ul>
        <p><strong>Example of Valid PAN:</strong> <code>AHGVE1276F</code></p>
    </div>

    <div class="section">
        <h2>📂 Categorisation</h2>
        <ul>
            <li><strong>Valid PAN:</strong> Matches all format and content rules.</li>
            <li><strong>Invalid PAN:</strong> Does not match the correct format, is incomplete, or contains non-alphanumeric characters.</li>
        </ul>
    </div>

    <div class="section">
        <h2>📝 Tasks Performed</h2>
        <ol>
            <li>Validated all PAN numbers based on the format rules.</li>
            <li>Separated the dataset into:
                <ul>
                    <li>✅ Valid PANs</li>
                    <li>❌ Invalid PANs</li>
                </ul>
            </li>
            <li>Generated a summary report.</li>
        </ol>
    </div>

    <div class="section">
        <h2>📊 Summary Report</h2>
        <ul>
            <li><strong>Total Records Processed:</strong> <code>[TO BE FILLED]</code></li>
            <li><strong>Total Valid PANs:</strong> <code>[TO BE FILLED]</code></li>
            <li><strong>Total Invalid PANs:</strong> <code>[TO BE FILLED]</code></li>
            <li><strong>Total Missing/Incomplete PANs:</strong> <code>[TO BE FILLED]</code></li>
        </ul>
    </div>

    <div class="section">
        <h3>📎 Dataset</h3>
        <p>The dataset used: <code>PAN_Number_Validation_Dataset.csv</code></p>
    </div>

    <footer>
        <p style="text-align: center; margin-top: 50px;">© 2025 PAN Validation Project • All Rights Reserved</p>
    </footer>

</body>
</html>
