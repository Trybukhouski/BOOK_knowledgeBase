# WEBPACK >> Extensions >> Dev-server

### Dev-server >> Install & Setup
1. Устанавливаемые плагины:
    - `webpack-dev-server` (-D)  
    Заносит изменения в оперативную память (не в dist) и обновляет страницу в режиме реального времени.
1. Создать новый узел в конфиг-файле:

    ```
    devServer: {
      port: 4200
    }
    ```
    - выбор порта опционален
1. Настроить package.json:

    ```
    script: {
      "start": "webpack-dev-server --mode development --open"
    }
    ```
1. Работа с сервером
    - Включить сервер:

      ```
      npm run start
      ```
    - Отключить сервер: 
      ```
      ctrl + C
      ```