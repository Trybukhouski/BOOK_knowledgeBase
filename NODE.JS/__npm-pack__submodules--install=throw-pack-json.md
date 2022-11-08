### __npm-pack
### __submodules 
### --install
### =throw-package.json
---
### Алгоритм
1. В файле `package.json` в объекте `dependencies` или `devDependencies` оставляем свойство вида:

    ```
    "moduleName": "1.2.2"
    ```
    - значение - это устанавливаемая версия в формате semver.
1. Ввести консольную команду:
    - Для модулей из `dependencies`:

      ```
      npm install
      ```
    - Для модулей из `devDependencies`:

      ```
      npm config
      ```