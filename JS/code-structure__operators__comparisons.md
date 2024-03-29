# COMPARISONS

## COMPARISONS >> About
- Операторы, использующиеся для сравнения двух операндов.
- Возвращают boolean.

## COMPARISONS >> List
- Больше / меньше: `>` / `<`
- Больше / меньше или равно: `=>` / `<=`
- Равно: `==`
- Не равно: `!=`

## COMPARISONS >> Rules >> String-operands
- Строки сравниваются посимвольно по unicode-кодировке.
- Большей становится тот операнд, который на одном индексе с вторым операндом имеет символ с бОльшим юникодом.
- Если все символы двух операндов имеют одинаковые юникоды на соответсвующих индексах, то они равны. Иначе большей считается более длинная строка.

## COMPARISONS >> Rules >> Different types operands
- Операторы приводятся к числу (по правилу приведения типов) и далее сравниваются числа.
- Если равенство строгое - приведение типов не производится.

## COMPARISONS >> Rules >> null & undefined
- При нестрогом равенстве равны друг другу, при строгом - не равны.
- Не равны никаким другим типам.

## COMPARISONS >> Rules >> NaN
- При сравнении на равенство NaN не равен ничему, даже самому себе.
- !?При сравнении через `>`, `<`, `<=`, `=>` всегда возвращает false.