\_\_ Resolve \_\_ Alias

# \_ Setup

1. Настраиваем пути в `alias`:

   ```
   resolve: {
     alias: {
       "@models": path.resolve(__dirname, 'src/models')
     }
   }
   ```

1. Переписываем пути в импорте модулей:

   ```
   import file.js from "./src/models/file.js"

   >>>

   import file.js from "@models/file.js"
   ```
