\_\_ Output-point

# \_ Setup

1. Создать объект output:

   ```
   output: {
     filename: null,
     path: path.resolve(__dirname, './dist')
   }
   ```

   - `filename` - файл(ы), в которые объединяются все JS-модули приложения.
   - `path` - место, КУДА надо складывать бандл-файл(ы).

1. Настроить файл точки выхода  
   **Вариант 1: Фиксированное имя**

   ```
     filename: 'bundle.js'
   ```

   - Подойдет в случаях, когда точка вывода одна.
   - Как правило, называется bundle.js (традиционное название).\

   **Вариант 2: Паттерны**

   ```
   [name].[contenthash].js
   ```

   - Подойдет в случаях, когда точек выхода несколько.
   - В этом случае следует настроить очистку dist, т.к. такая генерация файлов каждый раз генерирует новый, оставляя в папке старый "мусор".
   - Паттернов существует множество. Список [>>]()
