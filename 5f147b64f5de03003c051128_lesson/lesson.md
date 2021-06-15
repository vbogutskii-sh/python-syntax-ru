Часто возникает необходимость выполнить разные действия при выполнении разных условий. 

Условия (логические выражения) используются в операторах ветвления `if else`, в тернарном операторе и в циклах `for`, `while`.

**Условие** – это логическое (булево) выражение, которое может принимать значения `True` (истинно) или `False` (ложно). 

Условие состоит из двух выражений, соединенных операциями сравнения: 
`>` (больше), 
`<` (меньше), 
`<=` (меньше или равно), 
`>=` (больше или равно), 
`==` (равно), 
`!=` (не равно).

Например: 
```
x = 5
print(x > 0) # True (величина х положительна)
print(x >= 0); # True  (величина x неотрицательна)
print(x < 0); # False (величина х не является отрицательной)
print(15 == 3 * 5); # True  (значения равны)
print(15 != "15"); # True  (число 15 не равно строке "15")
```
Результатом логических выражений является значение типа bool (`True`  либо `False`). Название этому типу дано в честь британского математика Джорджа Буля.


**Составные условия** – это условия, которые состоят из двух или более простых условий, соединенных с помощью логических операторов И (`and`), ИЛИ (`or`) и НЕ (`not`).

И (`and`) используется в тех случаях, когда нужно проверить на истинность более одного условия.
```
if  условие and условие:
    действие

```
ИЛИ (`or`) используется тогда, когда мы хотим проверить на истинность хотя бы одно из двух и более условий.
```
if условие or условие:
    действие
```
НЕ (`not`) используется для отрицания.
```
if   not условие:
  действие
```
Условия в языке Python допускается записывать также с помощью двойных неравенств.

*Примеры*. Запишем на языке Python условия:
```
x > 9 and x <= 99 (число x – двухзначное положительное)
99 < x < 1000 (число x - трехзначное положительное)
type(x) == int (тип переменной х – integer)
address != "USA" (адрес не равен "USA")
not address == "USA" (адрес не равен "USA")
x == 6 or x == 7 (x равно одному из значений 6 или 7)
x % 2 == 0 and x % 3 == 0 (число x кратно 2 и 3)
name[0] in "AOIEU" (первая буква переменной name является заглавной гласной буквой)
not letter in "0123456789" (значение переменной letter не является цифрой)
month in [3,4,5]  # номер месяца равен 3, 4 или 5
```
Приоритет оператора И (`and`) больше, чем ИЛИ (`or`), поэтому он выполняется раньше. Например, 
```
a == 1 or b == 2 and b > c 
# Это условие равносильно следующему условию:
(a == 1) or (b == 2 and b > c)
```
Пример.
```
fruit = "banana"
print("a" in fruit)   # True
print("u" in fruit)   # False

vowels = "aeuio"
print("e" in vowels) # True
print("b" in vowels) # False
```