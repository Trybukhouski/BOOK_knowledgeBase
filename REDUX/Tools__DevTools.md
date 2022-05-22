# TOOLS >> DEVTOOLS

## Setup
1. Устанавливаем расширение для браузера:
    - __Chrome:__ Redux DevTools 
1. Устанавливаем в проект npm-пакет для devtools:

    ```
    npm install --save redux-devtools-extension
    ```
1. Импортируем из пакета необходимую функцию:  
    ```
    import {composeWithDevTools} from 'redux-devtools-extension'
    ```
1. -> Передаем импортированную функцию посленим аргументом в `createStore()`  
Особенности:
    - если в аргументах передавался `applyMiddleware()`, его необходимо передать не напрямую, аргументом в данную функцию.