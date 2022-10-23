# WEBPACK

### WP >> Setup >> Entry-point
- Если одна точка:

      ```
      entry: './address...'
      // ?или path.resolve(__dirname, './address...')
      ```
- Если несколько точек.  
  1. В `entry` указываем объект с полями-точками входа:

      ```
      entry: {
        main: './address...',
        secondPoint: './address...'
      }
      ```
    1. Настраиваем output для нескольких выходов.    
  Подробнее - в "output-point" [>>>]().