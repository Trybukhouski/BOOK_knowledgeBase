# REDUX-PERSIST

## About
- Это библиотека, которая позволяет гибко настраивать приложение через [ абстракцию ]? для синхронизации с Local-storage.
- Документация [>>](https://www.npmjs.com/package/redux-persist)

## Creation >> Basic
1. Имеем файл `configureStore.js`.  
Все последующие настройки будут производиться в нем.
1. Устанавливаем пакеты:
    - redux-persist

    Синтаксис:

    ```
    npm install redux-persist
    ```
1. Импортируем данные из установленной библиотеки:

    Name | Address | Info
    --- | --- | ---
    persistStore | redux-persist | обертка над `store`.
    persistReducer | redux-persist | преобразователь редюсеров.
    storage | redux-persist/lib/storage | хранилище
1. Создаем конфигурационный файл:
    ```
    const persistConfig = {
      key: 'root',
      storage,
    }
    ```
    - `storage` - это импортированый ранее storage.
    - `key` - настройка для создания нескольких хранилищ.

    Доп настройки:  
    [ ... ]
1. Создаем persistedReducer:
    - Создаем переменную `persistedReducer`
    - Присваиваем `persistedReducer` вызов импортированного метода `persistReducer()`
    - Передаем методу `persistReducer()` аргументами:
      - `persistConfig` - конфигурационный файл
      - `rootReducer` - наш основной редюсер

    Синтаксис:
    ```
    const persistedReducer = persistReducer(persistConfig, rootReducer)
    ```
1. В создаваемом `store` в передаваемом аргументе-объекте в поле `reducer` указываем `persistedReducer`.
1. Создаем persister

    Это [ ... ]  
    Алгоритм:

    - Определяем переменную `persistor`
    - Присваиваем `persistor` вызов импортированного метода `persistStore()` 
    - Передаем в `persistStore()` `store` приложения.

## Tutorial >> Black(white)list-settings
[ ... ]


## Tutorial >> React-integration
1. Производим basic-установку.
1. Импортируем данные в корневой файл реакт-приложения:

    Name | Adress | Info
    --- | --- | ---
    persistGate  | redux-persist/integration/react | Провайдер
    persistor | store-adress | ...
1. Оборачиваем приложение в импортированный провайдер `persistGate`
1. Передаем `persistGate` следующие атрибуты:
    - `loading`  
    Отвечает за прелоадер. Принимает реакт-компонент, либо null (если не требуется).
    - `persistor`  
    Принимает импортированный персистор.