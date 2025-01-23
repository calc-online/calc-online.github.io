<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Классический Калькулятор</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f0f0f0;
            user-select: none; /* Запрет выделения текста */
        }

        .calculator {
            border: 1px solid #ccc;
            border-radius: 10px;
            padding: 20px;
            background-color: #fff;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        #display {
            width: 100%;
            height: 70px; /* Высота поля ввода */
            text-align: right; /* Выравнивание текста вправо */
            font-size: 32px; /* Размер шрифта */
            margin-bottom: 10px;
            border: 1px solid #007bff; /* Синий цвет границы */
            border-radius: 5px;
            padding: 15px; /* Отступы внутри поля */
            background-color: #e9ecef; /* Светлый фон */
            color: #333; /* Цвет текста */
            box-shadow: inset 0 0 5px rgba(0, 0, 0, 0.2); /* Эффект глубины */
            box-sizing: border-box; /* Учитываем границы */
            outline: none; /* Убираем обводку */
            transition: all 0.3s ease; /* Плавное возвращение поля ввода в исходное положение */
        }

        .buttons {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 10px; 
        }

        button {
            height: 60px; /* Высота кнопки */
            width: 60px;  /* Ширина кнопки */
            font-size: 18px;
            cursor: pointer;
            border: none;
            border-radius: 50%;  /* Круглые кнопки */
            background-color: #007bff; /* Синий фон кнопок */
            color: white;
            transition: transform 0.1s ease; /* Плавный переход для эффекта анимации */
        }

        button:hover {
            background-color: #007bff; /* Оставляем тот же синий цвет при наведении */
        }

        button:active {
            transform: scale(0.9); /* Уменьшаем кнопку при нажатии */
        }

        h1 {
            margin-bottom: 20px; /* Отступ между заголовком и калькулятором */
            color: #333; /* Цвет текста заголовка */
        }

        /* Анимации для поля ввода */
        .shake {
            animation: shake 0.5s ease; /* Эффект потрясения */
        }

        .error {
            border-color: red; /* Красная граница при ошибке */
            background-color: #ffcccc; /* Красный фон при ошибке */
        }

        @keyframes shake {
            0% { transform: translateX(0); }
            25% { transform: translateX(-10px); }
            50% { transform: translateX(10px); }
            75% { transform: translateX(-10px); }
            100% { transform: translateX(0); }
        }

        /* Стиль для всплывающего уведомления */
        #notification {
            position: absolute;
            top: 20px;
            padding: 10px;
            background-color: #007bff;
            color: white;
            border-radius: 5px;
            display: none;
            font-size: 16px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            animation: fadeInOut 3s ease;
        }

        /* Стиль для таблички об успешной очистке */
        #clearedNotification {
            position: absolute;
            top: 90px;
            padding: 10px;
            background-color: #28a745; /* Зеленый фон */
            color: white;
            border-radius: 5px;
            display: none;
            font-size: 16px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            animation: fadeInOut 3s ease;
        }

        @keyframes fadeInOut {
            0% { opacity: 1; top: 20px; }
            50% { opacity: 1; top: 40px; }
            100% { opacity: 0; top: 60px; }
        }
    </style>
</head>
<body oncontextmenu="return false;">
    <h1>Калькулятор</h1> <!-- Заголовок -->

    <!-- Всплывающее уведомление -->
    <div id="notification">Нечего стирать!</div>

    <!-- Табличка об успешной очистке -->
    <div id="clearedNotification">Очищено</div>

    <div class="calculator">
        <!-- Поле ввода с type="tel" для вызова цифровой клавиатуры -->
        <input type="tel" id="display" oninput="validateInput()" pattern="[0-9]*" inputmode="numeric">

        <div class="buttons">
            <button onclick="clearDisplay()">C</button>
            <button onclick="backspace()">←</button> <!-- Кнопка для удаления одного символа -->
            <button onclick="appendToDisplay('/')">/</button>
            <button onclick="appendToDisplay('*')">*</button>
            <button onclick="appendToDisplay('7')">7</button>
            <button onclick="appendToDisplay('8')">8</button>
            <button onclick="appendToDisplay('9')">9</button>
            <button onclick="appendToDisplay('+')">+</button>
            <button onclick="appendToDisplay('4')">4</button>
            <button onclick="appendToDisplay('5')">5</button>
            <button onclick="appendToDisplay('6')">6</button>
            <button onclick="appendToDisplay('-')">-</button> <!-- Добавлена кнопка минуса -->
            <button onclick="calculateResult()">=</button>
            <button onclick="appendToDisplay('1')">1</button>
            <button onclick="appendToDisplay('2')">2</button>
            <button onclick="appendToDisplay('3')">3</button>
            <button onclick="appendToDisplay('0')">0</button>
            <button onclick="appendToDisplay('.')">.</button> <!-- Кнопка для точки -->
        </div>
    </div>

    <script>
        function validateInput() {
            const display = document.getElementById("display");
            const currentValue = display.value;
            // Регулярное выражение для проверки допустимых символов
            const allowedPattern = /^[0-9+\-*/.]*$/;

            // Если введенное значение не соответствует паттерну, очищаем поле ввода
            if (!allowedPattern.test(currentValue)) {
                display.value = ''; // Моментально удаляем текст
            }
        }

        function appendToDisplay(value) {
            const display = document.getElementById("display");
            display.value += value; // Добавляем символ в поле ввода
        }

        function clearDisplay() {
            const display = document.getElementById("display");
            if (display.value === '') {
                triggerShakeAndError();
                showNotification("Нечего стирать!");
            } else {
                display.value = ''; // Очищаем поле ввода
                showClearedNotification(); // Показать табличку "Очищено"
            }
        }

        function backspace() {
            const display = document.getElementById("display");
            if (display.value === '') {
                triggerShakeAndError();
                showNotification("Нечего стирать!");
            } else {
                display.value = display.value.slice(0, -1); // Удаляет последний символ
            }
        }

        function calculateResult() {
            const display = document.getElementById("display");
            try {
                display.value = eval(display.value); // Обрабатываем выражение
            } catch (error) {
                display.value = 'Ошибка'; // Если ошибка, выводим сообщение
            }
        }

        function triggerShakeAndError() {
            const display = document.getElementById("display");
            display.classList.add("shake", "error"); // Добавляем анимацию и красный стиль

            setTimeout(() => {
                display.classList.remove("shake", "error"); // Убираем классы после анимации
                display.style.backgroundColor = '#e9ecef'; // Восстановление фона
                display.style.borderColor = '#007bff'; // Восстановление цвета границы
            }, 500); // Время для анимации
        }

        function showNotification(message) {
            const notification = document.getElementById("notification");
            notification.textContent = message; // Устанавливаем текст уведомления
            notification.style.display = 'block'; // Показываем уведомление

            // Скрываем уведомление после 3 секунд
            setTimeout(() => {
                notification.style.display = 'none';
            }, 3000);
        }

        function showClearedNotification() {
            const clearedNotification = document.getElementById("clearedNotification");
            clearedNotification.style.display = 'block'; // Показываем уведомление

            // Скрываем уведомление после 3 секунд
            setTimeout(() => {
                clearedNotification.style.display = 'none';
            }, 3000);
        }
    </script>
</body>
</html>
