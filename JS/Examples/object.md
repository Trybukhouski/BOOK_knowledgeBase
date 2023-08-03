1. Обращение к имени свойства объекта через выражение

   ```
   let key = 'name';
   let user = {
    name: 'Ruslan'
   }
   user[key]   --->   'Ruslan'
   user.key   ---> undefined
   ```

1. Обращение к имени свойства объекта через выражение - практический пример

   ```
   let user = {
    name: 'Ruslan',
    age: 35,
   }

   let key = prompt('Какая информация вас интересует?', 'name');

   alert(user[key])
   ```
