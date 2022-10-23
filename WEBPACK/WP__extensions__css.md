# WEBPACK >> Extensions >> CSS

### CSS >> Install & Setup
1. Установить лоадеры:
    - `style-loader` 
    - `css-loader`
1. Указать правила в конфиг-файле:

    ```
    {
        test: /\.css$/,
        use: ['style-loader', 'css-loader']
    }
    ```
1. Импортировать главный CSS-файл в entry-файл:

    ```
    import '[address]'
    ``` 