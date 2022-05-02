# ELEMENT

## About
- Фрагмент кода, описывающий результат, который необходимо отобразить на экране.
- С точки зрения архитектуры, мельчайший кирпичик React-приложения.
- React-элемент - это простой JS-объект (не DOM-элемент).  
  До компиляции:

  ```
  const element = (
    <h1 className="greeting">
      Привет, мир!
    </h1>
  );
  ```
  После компиляции:

  ```
  const element = {
    type: 'h1',
    props: {
      className: 'greeting',
      children: 'Привет, мир!'
    }
  };
  ```

## Characteristics
- __Иммутабельный__  
После создания невозможно изменить:
  - его атрибуты
  - его потомков
- __Легковесный__  
Т.к. является обычным JS-объектом.

## Syntax >> Creation
<<<<<<< HEAD
Создать элемент можно двумя путями:
- Через DOM-tag
- Через React-компонент

## Syntax >> Creation from DOM-tag
  ```
  const element = <h1>Hello, world</h1>;
  ```
## Syntax >> Creation from React-component
=======

### Creation from DOM-tag
  ```
  const element = <h1>Hello, world</h1>;
  ```
### Creation from React-component
>>>>>>> 79ff31d41cc22f0141a789840a70d5ed830e0103

  ```
  const element = <Welcome name="Алиса" />
  ```
- Название компонента - это имя функции или класса, которая его объявляет.
- Классовый компонент вызывается без дополнительного определения объекта созданного класса.

## Syntax >> Rendering
- Подробности в модуле "rendering" >>>

## Draft
<<<<<<< HEAD
- Для отображения в UI элемент надо:
  - Создать.
  - Зарендерить в DOM-элемент.
- React-element можно сохранить в переменную:

  ```
  const elem = <h1>hi</h1>
  ```
=======

- Для отображения в UI элемент надо:
  - Создать.
  - Зарендерить в DOM-элемент.
>>>>>>> 79ff31d41cc22f0141a789840a70d5ed830e0103
