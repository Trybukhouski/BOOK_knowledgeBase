\_ Import

# -- Static fonts

1. Скачать в проект необходимые шрифты.
1. Установить лоадер:
   - `file-loader`
1. Указать правила в конфиг-файле:

   ```
   {
       test: /\.(ttf|woff|woff2|eot)$/,
       use: ['file-loader']
   }
   ```

   - Можно указать иные расширения в зависимости от используемых форматов шрифтов.

1. Импортировать шрифт в CSS-файл через стандартные CSS-средства (`@font-face`)
