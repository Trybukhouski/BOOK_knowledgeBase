# Creation >> Reducer

## Reducer
- Создается модуль rootReducer.js
- Создается функция `nameReducer`.
- В качестве аргументов в функцию передаются:
  - `state`  
  - `action`
- Функция всегда возвращает `state`.
- Внутри функции реализуется логика по изменению `state` на основании конкретного типа `action`:
  - Определение типа `action` происходит на основании поля `action.type`
  - В зависимости от значения `type` прописывается логика по изменению `state`.

## Reducer set
- Несколько редюсеров "объединяются" в единую сущность посредством встроенной в redux функции `combineReducers()`.  
Синтаксис:

  ```
  const rootReducer = combineReducers({
    firstReducerKey: firstReducer,
    seconfReducerKey: secondReducer
  })
  ```
  - Аргумент - это объект, хранящий поля с редюсерами под произвольными ключами.  
  Редюсеры в объекте вызывать не нужно.