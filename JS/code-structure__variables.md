# VARIABLES and CONSTANTS

# About
- Переменная - это именованное хранилище данных.

# Types
- Существует два вида переменных:
  - Изменяемая (переменная).
  - Неизменяемая (константа).  
  Попытка присвоить иное значение приведет к ошибке.

# Syntax
Тип|Инструкция|Имя|Оп-р присваивания|Данные
---|---|---|---|---
__Переменные:__ |let / var|camelCaseName|=|data
__Константы:__ |const|camelCaseName|=|data
- Повторное объявление переменной приведет к ошибке.

# Syntax >> Naming rules
- Имя должно содержать только буквы, цифры или символы $ и _.
- Первый символ не должен быть цифрой.
- Использовать верблюжью нотацию.
- Возможны любые языки.
- Имена регистрозависимы.
- Существуют зарезервированные имена, которые нельзя использовать.
- Для жестко закодированных, заранее известных значений - использовать константы с именами из заглавных букв (Пример: номер цвета)