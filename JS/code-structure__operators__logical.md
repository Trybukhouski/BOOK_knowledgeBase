# LOGICAL OPERATORS

## LOGICAL OPERATORS >> List
- Или: `||`
- И: `&&`
- Не: `!`
- Оп-р нулевого слияния: `??`

## LOGICAL OPERATORS >> About
- `!` - унарный оператор, а `&&`/`||` - тернарные.

## LOGICAL OPERATORS >> Rules
- Могут применяться к любым типам данных.
- Приоритетность:
  1. `!`
  1. `&&`
  1. `||`, `??`

## LOGICAL OPERATORS >> `||` >> About
- __С булевыми операндами__  
  - Возвращает true, если хотя бы один из операндов true.
- __С небулевыми операндами__
  - Возвращает первый логически truthy операнд, а если все операнды falsy - возвращает последний.

## LOGICAL OPERATORS >> `&&` >> About
- __С булевыми операндами__  
  - Возвращает false, если хотя бы один из операндов false.
- __С небулевыми операндами__
  - Возвращает первый логически falsy операнд, а если все операнды truthy - возвращает последний.

## LOGICAL OPERATORS >> `??` >> About
- Возвращает первый "определенный" операнд (не `null/undefined`), а если все операнды неопределены (`null/undefined`) - возвращает второй операнд.  
Т.е. похож на `||`/`&&`, но выводит не первое truthy/falsy, а первое определенное.

## LOGICAL OPERATORS >> `??` >> Rules
- Запрещено использовать с `||`/`&&` без скобок.
- Используется для:
  - Установка значения по умолчанию

    ```
    let a = null;
    a ?? 2 (Результат: 2);
    ```
  - Вывод первого определенного значения.

    ```
    let firstName = null;
    let lastName = undefined;
    let nickName = "Суперкодер";
    firstName ?? lastName ?? nickName (Результат: "Суперкодер")
    ```

## LOGICAL OPERATORS >> Rules >> `!`
- Приводит операнд к булевому типу согласно правилу приведения типов и возвращает обратное.