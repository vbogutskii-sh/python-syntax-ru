**find()** - поиск подстроки s в строке str. Возвращает номер первого вхождения или -1. Необязательные параметры `start`, `end`- позиции начала и конца поиска.
```
str.find(s, [start],[end])
```
**rfind()** - поиск подстроки s в строке str. Возвращает номер последнего вхождения или -1
```
str.rfind(s, [start],[end])
```
**index()** - поиск подстроки s в строке str. Возвращает номер первого вхождения или вызывает ValueError
```
str.index(s, [start],[end])
```
**rindex()** - поиск подстроки  s в строке str. Возвращает номер последнего вхождения или вызывает ValueError
```
str.rindex(s, [start],[end])
```
Также мы можем проверить, существует ли подстрока внутри строки или нет, используя ключевое слово `in`. 
```
print("a" in "apple") # True
```
Пример 1. 
```
word = "accessories"
i = word.find("a")
print(i)   # 0
print(word.find("s"))  # 4 (первое вхождение буквы "s" в строку word)
print(word.find("b"))  # -1 (буква "b" не найдена)
print(word.find("s", 6)) # 10 (при поиске буквы "s", начиная с индекса 6 до конца строки
print(word.find("s", 6, 9)) # -1 (при поиске буквы "s", начиная с 6 до 9 позиции, буква не найдена)
```

Пример 2. 
```
word = "september"
print(word.rfind("e")) # 7 (индекс последней буквы "e" в строке)
print(word.rfind("p"))  # 2 
print(word.rfind("a"))  # -1 (буква "a" не найдена)
```

Пример 3. 
```
word = "experience"
print(word.index("e")) # 0 (индекс первой буквы "e" в строке)
print(word.index("a"))  # ValueError: substring not found
```

Пример 4. 
```
word = "additional"
print(word.rindex("a")) # 8 (индекс последней буквы "a" в строке)
print(word.rindex("b"))  # ValueError: substring not found
```
Пример 5. 
```
text = "My flowers are nice"
print(text.index("nice")) # 15 (индекс вхождения  слова "nice" в строку text)
```
##### Задания
1. Создайте переменную word, присвойте ей значение "programmer". Найдите индекс первого и индекс последнего вхождения буквы "r" в строке word (используйте разные методы). 
1. Введите произвольную строку `s` и индекс `n`. Напечатайте n раз символ под индексом n. Например, если s = "computer", n = 3, то надо напечатать "ppp". 
1. Введите строку `full_name`, состоящую из имени и фамилии (например, "Bob Smith"), разделенных пробелом. Найти first_name и last_name и напечатать их с разных строках. 
1. Введите строку `string`, состоящую из двух слов, разделенных пробелом (например, "ice cream"). Получить и напечатать строку, в которой два слова поменялись местами: сначала второе слово, затем первое (например, "cream ice").
1. Введите строку `phrase`, состоящую из трех слов, разделенных пробелами (например, "Winter is Magic"). Получить и напечатать строку, в которой первое и последнее слово поменялись местами: сначала третье слово, затем второе и затем первое (например, "Magic is Winter").
1. Введите строку `text`, состоящую из трех слов, разделенных пробелами (например, "Enjoy every moment"). Получите второе слово, записанное в обратном порядке.
1. Создайте переменную `phrase` и присвойте ей значение "My eyes are green too!"
С помощью команды input спросите у пользователя "What is your favorite color? "
Замените слово "green" в переменной phrase на любимый цвет пользователя и напечатайте полученную фразу.
