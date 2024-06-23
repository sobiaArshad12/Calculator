<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Modern Calculator</title>
<style>
    body {
        font-family: 'Arial', sans-serif;
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        background-color: #f0f0f0;
        margin: 0;
    }
    .calculator {
        width: 300px;
        background-color: #fff;
        padding: 20px;
        border-radius: 8px;
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }
    #display {
        width: 100%;
        font-size: 2em;
        padding: 10px;
        text-align: right;
        border: 1px solid #ccc;
        border-radius: 4px;
        margin-bottom: 10px;
    }
    .buttons {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        gap: 10px;
    }
    button {
        font-size: 1.5em;
        padding: 15px;
        border: none;
        border-radius: 4px;
        cursor: pointer;
        background-color: #e0e0e0;
        transition: background-color 0.3s ease;
    }
    button:hover {
        background-color: #ccc;
    }
    .operator {
        background-color: #f0f0f0;
        font-weight: bold;
    }
    .operator:hover {
        background-color: #ddd;
    }
</style>
</head>
<body>
    <div class="calculator">
        <input type="text" id="display" placeholder="0" readonly>
        <div class="buttons">
            <button class="operator" data-value="/">÷</button>
            <button data-value="7">7</button>
            <button data-value="8">8</button>
            <button data-value="9">9</button>
            <button class="operator" data-value="*">x</button>
            <button data-value="4">4</button>
            <button data-value="5">5</button>
            <button data-value="6">6</button>
            <button class="operator" data-value="-">-</button>
            <button data-value="1">1</button>
            <button data-value="2">2</button>
            <button data-value="3">3</button>
            <button class="operator" data-value="+">+</button>
            <button data-value="0">0</button>
            <button data-value=".">.</button>
            <button id="equals" class="operator" data-value="=">=</button>
            <button id="clear">C</button>
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const display = document.getElementById('display');
            const buttons = document.querySelectorAll('button');

            buttons.forEach(button => {
                button.addEventListener('click', function() {
                    if (button.id === 'clear') {
                        clearDisplay();
                    } else if (button.id === 'equals') {
                        calculate();
                    } else {
                        addToDisplay(button.getAttribute('data-value'));
                    }
                });
            });

            function addToDisplay(value) {
                display.value += value;
            }

            function clearDisplay() {
                display.value = '';
            }

            function calculate() {
                try {
                    const result = eval(display.value);
                    display.value = Number.isInteger(result) ? result : result.toFixed(2); // Limit to 2 decimal places if necessary
                } catch (error) {
                    display.value = 'Error';
                }
            }
        });
    </script>
</body>
</html>
