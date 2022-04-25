# COMPONENT LIFELOOPS

## About
- Жизненные циклы:
  - Монтирование
  - Обновление
  - Размонтирование
  - Обработка ошибок

## ToDo
- Расписать все методы жизненных циклов.
- Разделить этапы жизненного цикла по отдельным файлам.



# MOUNTING

## About
- Этап создания компонента и его вставки в DOM.

## Methods
- `constructor()`
- `static getDerivedStateFromProps()`
- `render()`
- `componentDidMount()`

## ToDo
- Объединить раздел с creation




# UPDATE

## About
- Этап изменения пропсов или состояния.

## Methods
- `static getDerivedStateFromProps()`
- `shouldComponentUpdate()`
- `render()`
- `getSnapshotBeforeUpdate()`
- `componentDidUpdate()`



# UNMOUNTING

## About
- Этап удаления компонента из DOM.

## Methods
- `componentWillUnmount()`



# ОБРАБОТКА ОШИБОК

## About
- Этап, когда произошла ошибка в процессе рендеринга, методе жизненного цикла или конструкторе любого дочернего компонента.

## Methods
- `static getDerivedStateFromError()`
- `componentDidCatch()`
