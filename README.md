# 30-Days-Of-JavaScript

[_Day 2_](https://github.com/Asabeneh/30-Days-Of-JavaScript/blob/master/RU/02_Day/02_day_data_types.md#%f0%9f%93%94-day-2)

**Примитивные типы данных**(являются неизменяемыми типами данных)

_Числа (Numbers)_ - Целые числа, числа с плавающей точкой  
_Строки (Strings)_ - Любые данные в одинарных или двойных кавычках  
_Булевые (boolean)_ - true или false значения  
_Null_ - пустое значение или нет значения  
_Undefined_ - объявленная переменная без значения  

```
let numOne = 3;
let numTwo = 3;
console.log(numOne == numTwo); // true```
```

**Непримитивные типы данных**(являются изменяемыми)

_Объекты_  
_Функции_  
_Массивы_  

```
let nums = [1, 2, 3];
nums[0] = 10;
console.log(nums); // [10, 2, 3]
```

```
let nums = [1, 2, 3];
let numbers = [1, 2, 3];
console.log(nums == numbers); // false
```

**Математический объект**(Math Object- множество методов для работы с числами)

````
console.log(Math.round(9.81)); // 10 Округление до ближайшего числа если выше .5 вверх, если меньше 0.5 вниз  
console.log(Math.floor(PI)); // 3 округление вниз  
console.log(Math.ceil(PI)); // 4 округление вверх  
console.log(Math.min(-5, 3, 20, 4, 5, 10)); // -5, возвращает минимальное значение  
console.log(Math.max(-5, 3, 20, 4, 5, 10)); // 20, возвращает максимальное значение  
const randNum = Math.random(); // создаёт случайное число от 0 до 0,999999
console.log(randNum); //0.26794317623718245  
const num = Math.floor(Math.random() * 11); // создаёт случайное число от 0 до 10  
console.log(num);  
console.log(Math.abs(-10)); //10 Абсолютное значение  
console.log(Math.sqrt(100)); // 10 Квадратный корень  
console.log(Math.pow(3, 2)); // 9 (3 в квадрате)  
console.log(Math.log(2)); // 0.6931471805599453 Логарифм
console.log(Math.log(10)); // 2.302585092994046 Возвращает натуральный логарифм основания E из x, Math.log(x)  
Math.sin(0); //Тригонометрия
Math.cos(0);
````

**Генератор случайных чисел**

````
let randomNum = Math.random(); // генерирует от 0 до 0,999
let numBtnZeroAndTen = randomNum * 11;

console.log(numBtnZeroAndTen); // это даёт: мин 0 и макс 10.99

let randomNumRoundToFloor = Math.floor(numBtnZeroAndTen);
console.log(randomNumRoundToFloor); // это даёт от 0 до 10
````

**Конкатенация строк**

````
let space = " ";
let firstName = "Asabeneh";
let lastName = "Yetayeh";
let country = "Finland";
let city = "Helsinki";
let language = "JavaScript";
let job = "teacher";
let age = 250;
let fullName = firstName + space + lastName;

let fullName = firstName + space + lastName; // конкатенация, объединение двух строк.
console.log(fullName); // Asabeneh Yetayeh
let personInfoOne = fullName + ". I am " + age + ". I live in " + country;
console.log(personInfoOne); // Asabeneh Yetayeh. I am 250. I live in Finland
let personInfoTwo = `I am ${fullName}. I am ${age}. I live in ${country}.`; //ES6 - Метод строковой интерполяции

**Строковые Методы**

_length_: Метод строки length возвращает количество символов в строке, включая пустое пространство.  

````
let firstName = "Asabeneh";
console.log(firstName.length);
````

_Доступ к символам в строке_

````
let string = "JavaScript";
let lastIndex = string.length - 1;
console.log(lastIndex); // 9
console.log(string[lastIndex]); // t
````

_toUpperCase()_

````
let string = "JavaScript";
console.log(string.toUpperCase()); // JAVASCRIPT
````

_toLowerCase()_

````
console.log(string.toLowerCase()); // javascript
````

_substr()_(Требуется два аргумента: начальный индекс и количество символов для нарезки)

````
let string = "JavaScript";
console.log(string.substr(4, 6)); // Script (от 4го отрезать 6 символов)
````

_substring()_(Он принимает два аргумента: начальный индекс и индекс остановки, но он не включает индекс остановки)

````
let string = "JavaScript";
console.log(string.substring(0, 4)); // Java
console.log(string.substring(4, 10)); // Script
console.log(string.substring(4)); // Script
````

_split()_(разделяет строку в указанном месте)

````
let string = "30 Days Of JavaScript";

console.log(string.split()); // ["30 Days Of JavaScript"]
console.log(string.split(" ")); // ["30", "Days", "Of", "JavaScript"]

let firstName = "Asabeneh";

console.log(firstName.split()); // ["Asabeneh"]
console.log(firstName.split("")); // ["A", "s", "a", "b", "e", "n", "e", "h"]

let countries = "Finland, Sweden, Norway, Denmark, and Iceland";

console.log(countries.split(",")); // ["Finland", " Sweden", " Norway", " Denmark", " and Iceland"]
console.log(countries.split(", ")); //  ["Finland", "Sweden", "Norway", "Denmark", "and Iceland"]
````

_trim()_(Удаляет пробелы в начале или конце строки)

````
let string = "   30 Days Of JavaScript   ";
console.log(string.trim(" ")); // 30 Days Of JavasCript
````

_includes()_(Он проверяет, существует ли подстрока в строке, и возвращает true, если она существует, и false, если она не существует)

````
let country = "Finland";

console.log(country.includes("fin")); // false
console.log(country.includes("Fin")); // true
console.log(country.includes("land")); // true
console.log(country.includes("Land")); // false
````

_replace()_(принимает к параметру старую подстроку и новую подстроку)

````
let string = "30 Days Of JavaScript";
console.log(string.replace("JavaScript", "Python")); // 30 Days Of Python
````

_charAt()_(принимает индекс и возвращает значение по этому индексу)

````
let string = "30 Days Of JavaScript";
console.log(string.charAt(0)); // 3
````

_charCodeAt()_(Принимает индекс и возвращает код символа (номер ASCII) значения по этому индексу)

````
let string = "30 Days Of JavaScript";
console.log(string.charCodeAt(3)); // D ASCII number is 51
````

_indexOf()_(Принимает подстроку, и если подстрока существует в строке, она возвращает первую позицию подстроки, если не существует, она возвращает -1)

````
let string = "30 Days Of JavaScript";

console.log(string.indexOf("D")); // 3
console.log(string.indexOf("Days")); // 3
console.log(string.indexOf("days")); // -1
console.log(string.indexOf("a")); // 4
````

_lastIndexOf()_(Принимает подстроку, и если подстрока существует в строке, она возвращает последнюю позицию подстроки, если она не существует, она возвращает -1)

````
let string =
  "I love JavaScript. If you do not love JavaScript what else can you love.";

console.log(string.lastIndexOf("love")); // 67
console.log(string.lastIndexOf("you")); // 63
console.log(string.lastIndexOf("JavaScript")); // 38
````

_concat()_(он принимает множество подстрок и конкатенирует их)

````
let string = "30";
console.log(string.concat("Days", "Of", "JavaScript")); // 30DaysOfJavaScript
````

_startsWith_(он принимает подстроку в качестве аргумента и проверяет, начинается ли строка с указанной подстроки. Возвращает логическое значение (true или false).)

````
let string = "Love is the best to in this world";

console.log(string.startsWith("Love")); // true
console.log(string.startsWith("love")); // false
console.log(string.startsWith("world")); // false
````

_endsWith_(он принимает подстроку в качестве аргумента и проверяет, заканчивается ли строка указанной подстрокой. Возвращает логическое значение (true или false))

````
let string = "Love is the best to in this world";

console.log(string.endsWith("world")); // true
console.log(string.endsWith("love")); // false
console.log(string.endsWith("in this world")); // true
````

_search_(он принимает подстроку в качестве аргумента и возвращает индекс первого совпадения)

````
let string =
  "I love JavaScript. If you do not love JavaScript what else can you love.";
console.log(string.search("love")); // 2
````

_match_(он принимает подстроку или шаблон регулярного выражения в качестве аргумента и возвращает массив, если есть совпадение, если нет, то возвращает ноль. Давайте посмотрим, как выглядит шаблон регулярного выражения. Он начинается с / знака и заканчивается / знаком)

````
let string = "love";
let patternOne = /love/; //без какого-либо флага
let patternTwo = /love/gi; // g-означает поиск по всему тексту, i - без учета регистра
````

````
let string =
  "I love JavaScript. If you do not love JavaScript what else can you love.";
console.log(string.match("love")); // ["love", index: 2, input: "I love JavaScript. If you do not love JavaScript what else can you love.", groups: undefined]

let pattern = /love/gi;
console.log(string.match(pattern)); // ["love", "love", "love"]
````
Давайте извлечём числа из текста, используя регулярное выражение.

````
let txt =
  "In 2019, I run 30 Days of Python. Now, in 2020 I super exited to start this challenge";
let regEx = /\d+/;

// d с escape-символом означает, что d - не просто символ d, а обозначает цифру 
// + означает одно или несколько цифр,
// если после этого есть g, значит глобальный, ищите везде.

console.log(txt.match(regEx)); // ["2", "0", "1", "9", "3", "0", "2", "0", "2", "0"]
console.log(txt.match(/\d+/g)); // ["2019", "30", "2020"]
````

_repeat()_

````
let string = "love";
console.log(string.repeat(10)); // lovelovelovelovelovelovelovelovelovelove
````