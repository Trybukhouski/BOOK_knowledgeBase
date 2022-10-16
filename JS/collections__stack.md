# STACK

### STACK >> About >> Main
Базовое описание структуры >>>

### STACK >> Initialisation
```
let stack = []
```
- Стэк реализован через обычный js-массив.

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