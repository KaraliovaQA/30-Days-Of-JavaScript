# 30-Days-Of-JavaScript

Day 2

Примитивные типы данных(являются неизменяемыми типами данных)

Числа (Numbers) - Целые числа, числа с плавающей точкой
Строки (Strings) - Любые данные в одинарных или двойных кавычках
Булевые (boolean) - true или false значения
Null - пустое значение или нет значения
Undefined - объявленная переменная без значения

let numOne = 3;
let numTwo = 3;
console.log(numOne == numTwo); // true


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