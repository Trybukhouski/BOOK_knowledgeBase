\_ Import

# -- CSV

1. Установить лоадеры:

   - `papaparse`
   - `csv-loader`

1. Указать правила в конфиг-файле:

   ```
   {
       test: /\.(csv)$/,
       use: ['csv-loader']
   }
   ```

1. В импортируемом js-файле использовать команду импорта:

   ```
   import CSVFileName from "./.../CSVFileName.csv"
   ```
