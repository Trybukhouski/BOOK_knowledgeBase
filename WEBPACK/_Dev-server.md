# \_ Dev-server

1. Устанавливаем расширения:
   - `webpack-dev-server`  
     Заносит изменения в оперативную память (не в dist) и обновляет страницу в режиме реального времени.
1. Создаём новый объект в конфиг-файле:

   ```
   devServer: {
     port: 4200
   }
   ```

   - выбор порта опционален

1. Добавляем поле `start` в объекте `script` файла `package.json`:

   ```
   script: {
     "start": "webpack-dev-server --mode development --open"
   }
   ```

1. Запускаем сервер:

   ```
   npm run start
   ```

1. Отключаем сервер:

   ```
   ctrl + C
   ```
