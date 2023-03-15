\_\_ Resolve \_\_ Extensions

# \_ Setup

1. Указываем в массиве `extensions` список расширений по умолчанию:

   ```
   resolve: {
     extensions: ['.js', '.json', '.png']
   }
   ```

   - Если массив пустой, без указания расширения не распознаются никакие файлы.

1. 1. Переписываем пути в импорте модулей:

   ```
   import file from "./src/models/file.json"

   >>>

   import file from "./src/models/file"
   ```
