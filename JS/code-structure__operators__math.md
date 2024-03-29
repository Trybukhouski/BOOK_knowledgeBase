# MATH OPERATORS

## MATH OPERATORS >> list
- Сложение: `+`
- Вычитание: `-`
- Умножение: `*`
- Деление: `/`
- Взятие остатка от деления: `%`
- Возведение в степень: `**`

## MATH OPERATORS >> Features
- Инкремент / декремент
- Сокращенная арифметика с присваиванием
- Доп возможности `+`
  - Конкатенация строк
  - Приведение строк к числу

## MATH OPERATORS >> Features >> inc/de-crement
- Cинтаксис:

  ```
  counter++ (counter = counter + 1)
  counter-- (counter = counter - 1)
  ```
- Используется только с переменной, а не со значением.
- Имеет префиксную и постфиксную формы.

## MATH OPERATORS >> Features >> Сокращенная арифметика с присваиванием
- Cинтаксис:

  ```
  counter += 2 (counter = counter + 2)
  ```
- Механизм работает с любыми математическими и побитовыми операторами.

## MATH OPERATORS >> Features >> Доп возможности `+`
- __Конкатенация строк__  
При использовании оператора со строковыми операндами, произойдет их объединение в одну строку.
При этом если второй элемент конкатенации - не строка, то произойдет приведение к строке.
- __Приведение строк к числу__  
Синтаксис:

  ```
  +'1' = 1
  ```