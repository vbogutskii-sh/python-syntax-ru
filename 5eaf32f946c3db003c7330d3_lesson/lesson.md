**Операторы сравнения**

Операторы сравнения используются для сравнения значений. Они возвращают значения True или False.

Пусть заданы две переменные:
```
a = 10
b = 5
```

| Оператор  | Описание    |Пример      |
|----------------|------------------|----------------|
|> |больше. Возвращает True, если левый операнд больше правого| a > b  (10 > 5 ---> True)|
|<|меньше. Возвращает True, если левый операнд меньше правого| a < b  (10 < 5 ---> False)|
|>=|больше или равно. Возвращает True, если левый операнд больше или равен правому|a >= b (10 >= 5 ---> True)|
|<=|меньше или равно. Возвращает True, если левый операнд меньше или равен правому|a <= b (10 <= 5 ---> False)|
|==| равно. Возвращает True, если операнды равны|a == b  (10 == 5 ---> False)|
|!=|не равно. Возвращает True, если операнды не равны|a != b ( 10 != 5 ---> True)|

Примеры.
```
a = 10
b = 12

# Output: a > b is False
print('a > b is', a > b)

# Output: a < b is True
print('a < b is', a < b)

# Output: a == b is False
print('a == b is', a == b)

# Output: a != b is True
print('a != b is', a != b)

# Output: a >= b is False
print('a >= b is', a >= b)

# Output: a <= b is True
print('a <= b is', a <= b)
```
**Логические операторы**

Логические операторы and, or, not служат для записи составных условий, состоящих из двух и более операторов сравнений.
Пусть заданы логические переменные:
```
x = True
y = False
```

| Оператор  | Описание    |Пример      |
|----------------|------------------|----------------|
|and | Возвращает True, если оба операнда имеют значение True|   x and y  ---> False|
|or|Возвращает True, если хотя бы один из операндов имеет значение True| x or y ---> True)|
|not|Возвращает True, если операнд имеет значение False|not x ---> False|

Примеры.
```
a = 10
b = 12
print(a > 0 and b > 0)  # True and True ---> True
print(a < 0 and b > 0)  # False and True ---> False
print(a > 10 or b > 10) # False or True ---> True
print(a < 0 or b < 0)   # False or False ---> False
print(not a > 10)       # not True ---> False
print(not b < a)        # not False ---> True
 
```

##### Задания

1. Создайте переменную comp1, присвойте ей результат сравнения 3 > 2. Напечатайте значение переменной comp1.
2. Создайте переменную comp2, присвойте ей результат сравнения 3 < 2. Напечатайте значение переменной comp2.
3. Создайте переменную comp3, присвойте ей результат сравнения 2 >= 2. Напечатайте значение переменной comp3.
4. Создайте переменную comp4, присвойте ей результат сравнения 3 =< 5. Напечатайте значение переменной comp4.
5. Создайте переменную comp5, присвойте ей результат сравнения 2 == 2. Напечатайте значение переменной comp5.
5. Создайте переменную comp6, присвойте ей результат сравнения 2 != 5. Напечатайте значение переменной comp6.
