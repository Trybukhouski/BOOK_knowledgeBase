CSS >> Optimisation >> 

# DRY

### DRY >> Rules

- Повторяющиеся селекторы должны быть сгруппированы:

  ```
  h1 {
    color: #ff0000;
    font-family: Arial;
  }

  h2 {
    color: #ff0000;
    font-family: Arial;
  }

  >>>

  h1, h2 {
    color: #ff0000;
    font-family: Arial;
  }
  ```
- Повторяющиеся группы стилей следует объединять по схожему набору признаков и объединять в один класс.