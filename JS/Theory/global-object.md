- `Глобальный объект` - это js-объект, содержащий переменные и функции, доступные из любого места программы.
- `Глобальный объект` включает:
  - Встроенные в язык объекты (Array и др.)
  - Характерные для окружения свойства (innerHeight в браузере и др.)
- `Глобальное свойство` - это свойство, доступное всем скриптам программы.  
  ..| А будет ли оно доступно модуле 1, если записано в `глобальный объект` в модуле 2? |
- По умолчанию глобальный объект содержит методы и функции, изначально встроенные в язык или среду исполнения.
- ..| Глобальный объект есть в любой среде исполнения JS-кода |
- `window` - название `глобального объекта` в браузере.
- `global` - название `глобального объекта` в Node.js.
- `globalThis` - стандартизированное имя `глобального объекта` для всех сред исполнения JS-кода.
- `Function Declaration` содержит ключевое слово `function` в основном потоке кода.
- `Полифил` - самописная функция, которая не поддерживается окружением, но существует в современном стандарте.