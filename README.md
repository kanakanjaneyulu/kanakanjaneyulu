<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tax Calculator</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <h1>Tax Calculator</h1>
        <form id="taxForm">
            <div class="form-group">
                <label for="age">Age:</label>
                <select id="age" class="input-field" required>
                    <option value="<40">&lt; 40</option>
                    <option value=">=40 & <60">&ge; 40 &lt; 60</option>
                    <option value=">=60">&ge; 60</option>
                </select>
            </div>
            <div class="form-group">
                <label for="income">Income (in Lakhs):</label>
                <input type="number" id="income" class="input-field" required>
                <div class="error-icon" id="income-error" style="display: none">!</div>
            </div>
            <div class="form-group">
                <label for="deductions">Deductions (in Lakhs):</label>
                <input type="number" id="deductions" class="input-field">
                <div class="error-icon" id="deductions-error" style="display: none">!</div>
            </div>
            <button type="submit" id="submitBtn">Submit</button>
        </form>
    </div>
    <div id="modal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <h2>Final Tax Calculation</h2>
            <div id="result"></div>
        </div>
    </div>
    <script src="script.js"></script>
</body>
</html>
age) {
        switch (age) {
            case '<40':
                return 0.3;
            case '>=40 & <60':
                return 0.4;
            case '>=60':
                return 0.1;
            default:
                return 0;
        }
    }
});
