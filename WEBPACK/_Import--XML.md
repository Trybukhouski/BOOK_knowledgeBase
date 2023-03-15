\_ Import

# -- XML

1. Установить лоадер:
   - `xml-loader`
1. Указать правила в конфиг-файле:

   ```
   {
       test: /\.(xml)$/,
       use: ['xml-loader']
   }
   ```

1. В импортируемом js-файле использовать команду импорта:

   ```
   import XMLFileName from "./.../XMLFileName.xml"
   ```
