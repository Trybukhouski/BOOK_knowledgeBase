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

### Creation from DOM-tag
  ```
  const element = <h1>Hello, world</h1>;
  ```
### Creation from React-component

  ```
  const element = <Welcome name="Алиса" />
  ```

## Draft

- Для отображения в UI элемент надо:
  - Создать.
  - Зарендерить в DOM-элемент.