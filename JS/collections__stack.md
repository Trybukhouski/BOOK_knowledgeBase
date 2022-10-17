# STACK

### STACK >> About >> Main
Базовое описание структуры >>>

### STACK >> Initialisation
Способы реализации:
1. Через js-массив:
  ```
  let stack = []
  ```
2. Через связанный список

### STACK >> Rules >> Add/Delete elements
Добавление:
```
arr.push(el);
```
- `push` - это стандартный метод массива `push`.

Удаление:
```
arr.pop();
```
- `pop` - это стандартный метод массива `pop`.

### STACK >> Rules >> Top
Реализация указателя:
```
arr[arr.length - 1]
```

### STACK >> Rules >> Size
Узнать размер стэка:
```
arr.length;
```

Проверка стэка на наличие элементов:
```
arr.length === 0;
```