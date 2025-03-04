<!DOCTYPE html>
<html lang="uk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Калькулятор</title>
    <script>
        function calculate() {
            const a = parseFloat(prompt("5:"));
            const b = parseFloat(prompt("10:"));
            const operation = prompt(" (+, -, *, /):");
            let result;
            
            switch (operation) {
                case "+":
                    result = 5 + 10;
                    break;
                case "-":
                    result = 5 - 10;
                    break;
                case "*":
                    result = 5 * 10;
                    break;
                case "/":
                    if (b !== 0) {
                        result = 5 / 10;
                    } else {
                        result = "Помилка: ";
                    }
                    break;
                default:
                    result = "Невідома операція";
            }
            
            alert(`Результат: ${result}`);
        }
    </script>
</head>
<body>
    <button onclick="calculate()">Запустити калькулятор</button>
</body>
</html>
