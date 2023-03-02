# 30-Days-Of-JavaScript

[_Day 2_](https://github.com/Asabeneh/30-Days-Of-JavaScript/blob/master/RU/02_Day/02_day_data_types.md#%d0%a3%d0%bf%d1%80%d0%b0%d0%b6%d0%bd%d0%b5%d0%bd%d0%b8%d0%b5-%d0%a3%d1%80%d0%be%d0%b2%d0%b5%d0%bd%d1%8c-1)

Примитивные типы данных(являются неизменяемыми типами данных)

Числа (Numbers) - Целые числа, числа с плавающей точкой
Строки (Strings) - Любые данные в одинарных или двойных кавычках
Булевые (boolean) - true или false значения
Null - пустое значение или нет значения
Undefined - объявленная переменная без значения

```let numOne = 3;
let numTwo = 3;
console.log(numOne == numTwo); // true```


Непримитивные типы данных(являются изменяемыми)

Объекты
Функции
Массивы

let nums = [1, 2, 3];
nums[0] = 10;
console.log(nums); // [10, 2, 3]

let nums = [1, 2, 3];
let numbers = [1, 2, 3];
console.log(nums == numbers); // false