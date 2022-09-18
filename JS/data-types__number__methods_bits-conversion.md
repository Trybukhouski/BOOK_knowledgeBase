# Numeral systems conversion

### NUM CONVERSION >> X-bits -> 10-bits
- 2-bits:

  ```
  0b101 -> 5
  ```
- 8-bits:

  ```
  0o456 -> 302
  ````
- 16-bits:

  ```
  0xff -> 255
  ```
- other systems:

  ```
  parseInt(num, num-system)
  ```

### NUM CONVERSION >> 10-bits -> X-bits
- В 2-36 битов:

  ```
  10-bit-num.toString(num-system)
  ```
  - Возвращает строковое представление.
  - При вызове на числе (а не на переменной) - необходимо вызывать метод через две точки, либо обернуть число в (скобки).