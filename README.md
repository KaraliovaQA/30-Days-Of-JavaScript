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