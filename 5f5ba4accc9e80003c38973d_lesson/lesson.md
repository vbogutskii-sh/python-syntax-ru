Метод `split()` разбивает строку на массив подстрок путём разделения строки указанным разделителем. Возвращаемое значение – массив строк, которые получатся, если исходную строку разрезать на части по символам-разделителям. При этом исходная строка остается неизменной.

Синтаксис: 
```
lst = string.split(separator)
```
Здесь где separator – символ, который используется в качестве разделителя. Разделитель - необязательный параметр. Если разделитель не указывается, то строка разбивается на подстроки по пробелам.

Пример 1.
```
s = "Sky is orange today"
lst = s.split()  # разделитель отсутствует, строка разбивается по пробелам
print(lst) # ["Sky", "is",  "orange", "today"]
```
Пример 2.
```
time = "12:15:30"
lst = time.split(":")  # строка разбивается по двоеточиям
print(lst) # ["12", "15",  "30"]
```
Но если вам надо слово разбить на отдельные буквы, то следует преобразовывать слово в массив с помощью функции list():
```
word = "hello"
letters = list(word)
print(letters)  # ["h", "e", "l", "l", "o"]
```