optimisation >> DRY >>

### Rules
Для избавления от дублирующей логики, в зависимости от ситуации, можно:
- Использовать циклы

  ```
  console.log('corn');
  console.log('pita');
  console.log('potato');
  console.log('tortilla');

  >>>

  const chips = ['corn', 'pita', 'potato', 'tortilla'];
  for ( let i = 0; i < chips.length; i++) {
  console.log(chips[i]);
  }
  ```
  - ..[Метод подойдет, когда повторяющаяся логика повторяется среди сестринских DOM-узлов]
- Использовать функции
  - ..[Метод подойдет, когда повторяющаяся логика содержится в различных местах кода]