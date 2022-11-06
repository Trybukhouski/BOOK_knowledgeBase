# FABRIC MODULE

### FABRIC MOD >> About >> Main
Модуль-фабрика - это разновидность модуля, который содержит параметры при его импорте в другие модули.

### FABRIC MOD >> Rules >> Syntax
1. Экспортирование модуля-фабрики:

    ```
    module.exports = function(par-1[, par-2, etc...]) {
      return function() {
        //code
      }
    }
    ```
1. Импортирование модуля-фабрики:

    ```
    let name = require('./address/modName')(arg-1[, arg-2, etc...])
    ```
1. Используйте импортированный модуль с переданными параметрами.