# \_ SCSS-install

1. Установить лоадеры:
   - `node-sass`
   - `sass-loader`
1. Указать правила в конфиг-файле:

   ```
   {
       test: /\.s[ac]ss$/,
       use: ['style-loader', 'css-loader', 'sass-loader']
   }
   ```

1. Импортировать главный SCSS-файл в entry-файл:

   ```
   import '[address]'
   ```
