# CONVERSION

# CONVERSION >> About
- Преобразование осуществляется двумя способами:
  - Автоматическое
  - Явное

# CONVERSION >> To String >> Rules
- Происходит очевидным способом.  
Пример:

  ```
  null -> 'null'
  false -> 'false'
  ```

# CONVERSION >> To String >> Syntax
- Явно
  - через `String(value)`

    ```
    String(value)
    ```
- Автоматически
  - через `alert(value)`

    ```
    alert(value)
    ```

# CONVERSION >> To Number >> Rules
- undefined ->	NaN  
- null	-> 0  
- true / false	-> 1 / 0
- string ->
  - Пустая строка -> 0, 
  - '6' -> 6
  - 'six' -> NaN  
  - Пробельные символы по краям обрезаются. 

# CONVERSION >> To Number >> Syntax
- Явно
  - через `Number(value)`

    ```
    Number(value)
    ```
- Автоматически
  - через математические операторы

    ```
    6 / '2' -> 3
    6 / 'two' -> NaN
    ```

# CONVERSION >> To Boolean >> Rules
- Все значения, кроме интуитивно пустых -> true
- Интуитивно пустые значения -> false
  - 0
  - пустая строка (и только!)
  - null
  - undefined
  - NaN

# CONVERSION >> To Boolean >> Syntax

- Явно
  - через `Boolean(value)`

    ```
    Boolean(value)
    ```
- Автоматически
  - через логические операции