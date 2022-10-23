# WEBPACK >> Extensions >> Dist-cleaning

### Dist-cleaning >> Install & Setup
1. Устанавливаемые плагины: 
    - `clean-webpack-plugin` (-D)
1. Нюансы установки:  
    - Импортировать плагин в конфиг-файл следует через деструктуризацию:

      ```
      const {CleanWebpackPlugin} = ...
      ```