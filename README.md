<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body style="font-family: 'Times New Roman', Times, serif;">
    <p align = "center" style="font-size: 14;">
        МИНИСТЕРСТВО НАУКИ И ВЫСШЕГО ОБРАЗОВАНИЯ <br>
        РОССИЙСКОЙ ФЕДЕРАЦИИ<br>
        ФЕДЕРАЛЬНОЕ ГОСУДАРСТВЕННОЕ БЮДЖЕТНОЕ<br>
        ОБРАЗОВАТЕЛЬНОЕ УЧРЕЖДЕНИЕ ВЫСШЕГО ОБРАЗОВАНИЯ<br>
        «САХАЛИНСКИЙ ГОСУДАРСТВЕННЫЙ УНИВЕРСИТЕТ»<br>
    </p>
    <br><br><br><br><br><br>
    <body font-size = "12">
        <p align = "center"> 
            Институт естественных наук и техносферной безопасности<br>
            Кафедра информатики<br>
            Бахтина Елена Владимировна<br>
        </p>
        <br><br><br>
        <p align = "center">
            <strong>Лабораторная работа №10. «JavaScript».</strong><br>
            01.03.02 Прикладная математика и информатика
        </p>
        <br><br><br><br><br><br><br><br><br><br><br><br>
        <p align = "right"> 
            Научный руководитель<br>
            Соболев Евгений Игоревич
        </p>
        <br><br><br>
        <p align = "center">г. Южно-Сахалинск<br>2024 г.</p>
    </body>
    <body style="font-family: 'Times New Roman', Times, serif;">
        <h2 align = "center">Введение</h2>
        <p font-size = "12">
            <b>JavaScript</b> — мультипарадигменный язык программирования. Поддерживает объектно-ориентированный, императивный и функциональный стили.
        </p>
        <br>
        <h2 align = "center">Цель и задачи</h2>
        <p align = "left" font-size = "12"> 
            Цель: решить задачи при помощи JS.<br>
            Задачи:<br>
                1.	Напишите функцию, которая найдёт числа в массиве, которые делятся на заданное число. <br>
                2.	Нужно написать функцию, которая проверяет, являются ли две строки анаграммами, причем регистр букв не имеет значения. Учитываются лишь символы; пробелы или знаки препинания в расчет не берутся.<br>
                3.	Нужно написать функцию, принимающую строку в качестве аргумента и возвращающую количество гласных, которые содержатся в строке.
                Гласными являются «a», «e», «i», «o», «u».<br>
                4.	Треугольник. Напишите цикл,  выводит такой треугольник:<br>
                #<br>
                ##<br>
                ###<br>
                ####<br>
                #####<br>
                ######<br>
                #######<br>
                5.	FizzBuzz. Напишите программу, которая выводит через console.log все числа от 1 до 100, с двумя исключениями. Для чисел, нацело делящихся на 3, она должна выводить ‘Fizz’, а для чисел, делящихся на 5 (но не на 3) – ‘Buzz’.Когда сумеете – исправьте её так, чтобы она выводила «FizzBuzz» для всех чисел, которые делятся и на 3 и на 5.<br>
                6.	Шахматная доска. Напишите программу, создающую строку, содержащую решётку 8х8, в которой линии разделяются символами новой строки. На каждой позиции либо пробел, либо #. <br>
                7.	Минимум. Напишите функцию min, принимающую два аргумента, и возвращающую минимальный из них.<br>
                8.	Рекурсия. Ноль чётный. Единица нечётная. У любого числа N чётность такая же, как у N-2. Напишите рекурсивную функцию isEven согласно этим правилам. Она должна принимать число и возвращать булевское значение. Потестируйте её на 50 и 75. Попробуйте задать ей -1. Почему она ведёт себя таким образом? Можно ли её как-то исправить?<br>
                9.	Считаем бобы. Символ номер N строки можно получить, добавив к ней .charAt(N) ( “строчка”.charAt(5) ) – схожим образом с получением длины строки при помощи .length. Возвращаемое значение будет строковым, состоящим из одного символа (к примеру, “к”). У первого символа строки позиция 0, что означает, что у последнего символа позиция будет string.length – 1. Другими словами, у строки из двух символов длина 2, а позиции её символов будут 0 и 1.Напишите функцию countBs, которая принимает строку в качестве аргумента, и возвращает количество символов “B”, содержащихся в строке.Затем напишите функцию countChar, которая работает примерно как countBs, только принимает второй параметр — символ, который мы будем искать в строке (вместо того, чтобы просто считать количество символов “B”). Для этого переделайте функцию countBs.<br>
                10.	Сумма диапазона.  Напишите функцию range, принимающую два аргумента, начало и конец диапазона, и возвращающую массив, который содержит все числа из него, включая начальное и конечное.Затем напишите функцию sum, принимающую массив чисел и возвращающую их сумму. Запустите указанную выше инструкцию и убедитесь, что она возвращает 55.В качестве бонуса дополните функцию range, чтобы она могла принимать необязательный третий аргумент – шаг для построения массива. Если он не задан, шаг равен единице. Вызов функции range(1, 10, 2) должен будет вернуть [1, 3, 5, 7, 9]. Убедитесь, что она работает с отрицательным шагом так, что вызов range(5, 2, -1) возвращает [5, 4, 3, 2].<br>
                11.	Обращаем массив вспять. Напишите две функции, reverseArray и reverseArrayInPlace. Первая получает массив как аргумент и выдаёт новый массив, с обратным порядком элементов. Вторая работает как оригинальный метод reverse – она меняет порядок элементов на обратный в том массиве, который был ей передан в качестве аргумента. Не используйте стандартный метод reverse.<br>
                12.	Глубокое сравнение. Оператор == сравнивает переменные объектов, проверяя, ссылаются ли они на один объект. Но иногда полезно было бы сравнить объекты по содержимому. Напишите функцию deepEqual, которая принимает два значения и возвращает true, только если это два одинаковых значения или это объекты, свойства которых имеют одинаковые значения, если их сравнивать рекурсивным вызовом deepEqual. Чтобы узнать, когда сравнивать величины через ===, а когда – объекты по содержимому, используйте оператор typeof. Если он выдаёт “object” для обеих величин, значит нужно делать глубокое сравнение. Не забудьте об одном дурацком исключении, случившемся из-за исторических причин: “typeof null” тоже возвращает “object”.<br>
                13.	Свертка. Используйте метод reduce в комбинации с concat для свёртки массива массивов в один массив, у которого есть все элементы входных массивов.
        </p>
        <h2 align = "center">Решение</h2>
        <p font-size = "12">Для выполнения этой лабораторной работы, я пользовалась:</p>
        <p> 1.  Материалом в сети интернет</p>
        </body>
<h3 align = "center">Файл lab10.html</h3>

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>lab10</title>
</head>
<body>
    <div>
        <p class="title">Первое задание:</p>
        <p id="first"></p>
        <p class="title">Второе задание:</p>
        <p id="second"></p>
        <p class="title">Третье задание:</p>
        <p id="third"></p>
        <p class="title">Четвертое задание:</p>
        <p id="fourth"></p>
        <p class="title">Пятое задание:</p>
        <a href="https://www.programiz.com/javascript/online-compiler/">проверка кода</a>
        <p class="title">Шестое задание:</p>
        <p id="Sixth"></p>
        <p class="title">Седьмое задание:</p>
        <p id="seventh"></p>
        <p class="title">Восьмое задание:</p>
        <p id="eight"></p>
        <p class="title">Девятое задание:</p>
        <p id="nine"></p>
        <p class="title">Десятое задание:</p>
        <p id="ten"></p>
        <p class="title">Одинадцатое задание:</p>
        <p id="eleven"></p>
        <p class="title">Двенадцатое задание:</p>
        <p id="twelve"></p>
        <p class="title">Тринадцатое задание:</p>
        <p id="thirteen"></p>
    </div>
    <script>
        function findnum(arr, divisor) {
            return arr.filter(num => num % divisor === 0);
        }
        const numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
        const divisor = 3;
        const result = findnum(numbers, divisor);
        document.getElementById('first').innerText = `Числа, которые делятся на ${divisor}: ${result}`;
    </script>
    <script>
        function anagran(str1, str2) {
            const mystring = function(str) {
                return str.toLowerCase().replace(/[^а-я]/g, '').split('').sort().join('');
            }
            const mystring1 = mystring(str1);
            const mystring2 = mystring(str2);
            return mystring1 === mystring2;
        }
        const string1 = 'нос';
        const string2 = 'сон';
        if (anagran(string1, string2)) {
           document.getElementById('second').innerText = `${string1} и ${string2} являются анаграммами`;
        } else {
            document.getElementById('second').innerText = `${string1} и ${string2} не являются анаграммами`;
        }
    </script>
    <script>
        function count(str) {
            str = str.toLowerCase();
            const vowels = /[aeiou]/g;
            const vowelsCount = str.match(vowels) ? str.match(vowels).length : 0;
            return vowelsCount;
        }
        const inputString = 'chupapi munyanya';
        const vowelsCount = count(inputString);
        document.getElementById('third').innerText = `Количество гласных в строке ${inputString} равно: ${vowelsCount}`;
    </script>
    <script>
        function drawTriangle(n) {
            let row = '';
            for (let i = 1; i <= n; i++) {
                row = '\n';
                for (let j = 1; j <= i; j++) {
                    row += '#';
                }
                document.getElementById('fourth').innerText += `${row}`;
            }
        }
        drawTriangle(6);
    </script>
    <script>
        function FizzBuzz()
        {
            for (let i = 1; i <= 100; i++) {
                if (i % 3 === 0 && i % 5 === 0) {
                    console.log('FizzBuzz');
                } else if (i % 3 === 0) {
                    console.log('Fizz');
                } else if (i % 5 === 0) {
                    console.log('Buzz');
                } else {
                    console.log(i);
                }
            }
        }
    </script>
    <script>
        let size = 8;
        let board = '';
        for (let i = 0; i < size; i++) {
            for (let j = 0; j < size; j++) {
                if ((i + j) % 2 === 0) {
                    board += '__';
                } else {
                    board += '#';
                }
            }
            board += '\n';
        }
        document.getElementById('Sixth').innerText = `${board}`;
    </script>
    <script>
        function min(a, b)
        {
            if (a < b) {return a;}
            else {return b;}
        }
        document.getElementById('seventh').innerText = `${min(1, 3)}`;
    </script>
    <script>
        function isEven(number) {
            if (number < 0) {
                return isEven(-number);
            }
            if (number === 0) {
                return true;
            } else if (number === 1) {
                return false;
            } else {
                return isEven(number - 2);
            }
        }
        document.getElementById('eight').innerText = `Если 50: ${isEven(50)}\n Если 75: ${isEven(75)}\n Если -1: ${isEven(-1)}`;
    </script>
    <script>
        function countBs(str) {
            let count = 0;
            for (let i = 0; i < str.length; i++) {
                if (str.charAt(i) === 'B') {
                    count++;
                }
            }
            return count;
        }
        function countChar(str, char) {
            let count = 0;
            for (let i = 0; i < str.length; i++) {
                if (str.charAt(i) === char) {
                    count++;
                }
            }
            return count;
        }
        let test = "Bean bean Bee";
        document.getElementById('nine').innerText = `Если countBs(Bean bean Bee): ${countBs(test)}\n Если countChar(Bean bean Bee, B): ${countChar(test, 'B')}`;
    </script>
    <script>
        function range(start, end, step = 1) {
            let result = [];
            if (step > 0) {
                for (let i = start; i <= end; i += step) {
                    result.push(i);
                }
            } else {
                for (let i = start; i >= end; i += step) {
                    result.push(i);
                }
            }
            return result;
        }
        function sum(numbers) {
            let total = 0;
            for (let number of numbers) {
                total += number;
            }
            return total;
        }
        document.getElementById('ten').innerText = `Массив от 1 до 10 с шагом 2:\n${range(1, 10, 2)}\nМассив от 5 до 2 с шагом -1:\n${range(5, 2, -1)}\nСумма массива от 1 до 10:\n${sum(range(1, 10))}`;
    </script>
    <script>
        function reverseArray(arr) {
            let newar = [];
            for (let i = arr.length - 1; i >= 0; i--) {
                newar.push(arr[i]);
            }
            return newar;
        }
        function reverseArrayInPlace(arr) {
            for (let i = 0; i < Math.floor(arr.length / 2); i++) {
                let temp = arr[i];
                arr[i] = arr[arr.length - 1 - i];
                arr[arr.length - 1 - i] = temp;
            }
            return arr;
        }
        let arr = [1, 2, 3, 4, 5];
        document.getElementById('eleven').innerText = `reverseArray массив от 1 до 5: ${reverseArray(arr)}\reverseArrayInPlace массив от 1 до 5: ${reverseArrayInPlace(arr)}`;
    </script>
    <script>
        function deepEqual(a, b) {
            if (a === b) {
                return true;
            }
            if (a == null || typeof a !== 'object' || b == null || typeof b !== 'object') {
                return false;
            }
            let keysA = Object.keys(a);
            let keysB = Object.keys(b);
            if (keysA.length !== keysB.length) {
                return false;
            }
            for (let key of keysA) {
                if (!keysB.includes(key) || !deepEqual(a[key], b[key])) {
                    return false;
                }
            }
            return true;
        }
        let arr1 = [1, 2, 3];
        let arr2 = [1, 2, 3];
        let arr3 = [1, 2, 4];
        document.getElementById('twelve').innerText = `${deepEqual(arr1, arr2)} ${deepEqual(arr1, arr3)}\n`;
        let value1 = 42;
        let value2 = 42;
        let nul = null;
        document.getElementById('twelve').innerText += `${deepEqual(value1, value2)} ${deepEqual(nul, null)}`;
    </script>
    <script>
        let arrr = [[1, 2], [3, 4], [5, 6]];
        let newar = arrr.reduce((acc, curar) => acc.concat(curar), []);
        document.getElementById('thirteen').innerText = `${newar}`;
    </script>
</body>
</html>
```
</html>
<br>
 <h2 align = "center">Вывод</h2>
 <p align = "left" font-size = "12">
    По итогу данной лабороторной работы, я научилась новым интересным вещам на этом язке 😊 
</p>
</body>
</html>
