\_ Import

# -- Static images

1. Установить лоадер:
   - `file-loader`
1. Указать правила в конфиг-файле:

   ```
   {
       test: /\.(png|jpg|svg|gif)$/,
       use: ['file-loader']
   }
   ```

   - можно указать иные расширения в зависимости от используемых форматов файлов.

1. Вставить в файл (CSS или JS)  
   CSS:
   ```
   .selector {
      background-image: url("./.../imageName.png")
   }
   ```
   JS:
   ```
   import imageName from "./.../imageName.png"
   ```
