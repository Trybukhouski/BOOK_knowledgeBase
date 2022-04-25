# RENDERING

## About
...

## Types
- __..Непосредственный..__
- __Условный рендеринг__  
Выбор варианта отоборжаения изменений в зависимости от прописанного условия.
- __..Самообновление..__

## Syntax
- Виды рендеринга:
  - Рендеринг в DOM
  - Рендеринг в другой компонент

## Syntax >> Rendering into DOM
```
ReactDOM.render(React-elem, DOM-elem[, callback])
```
- `ReactDOM` - это...
- `render()` - метод для рендеринга React-элемента в DOM-элемент.  
?Возвращает ссылку на компонент. Если у компонента нет состояния - `null`.?
- `React-elem` - React-элемент, который мы рендерим в DOM-узел.
- `DOM-elem` - DOM-узел, в который мы рендерим React-элемент.
- `callback` - коллбэк-функция, которая вызовется после того, когда компонентся отрендерится или обновится.

## Syntax >> Rendering into other component
...

## ToDo
- Определение "Рендеринг"
- Рендеринг в другой компонент
- Заполнить пункт "самообновление"