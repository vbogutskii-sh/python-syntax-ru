Циклы можно использовать, чтобы по очереди перебрать все элементы строки. 

##### Цикл **for ... in range():**
Синтаксис команды:
```
for <index> in range(len(string)):
    <operator>
```
Здесь `index` - переменная, обозначающая индекс элемента строки;
`len(string)` - длина строки с именем string; `operator` - одна или несколько команд, которые выполняются в цикле.

Пример 1. Напечатать все символы строки x = "hello" по одному в строке.
```
x = "hello" 
for i in range(len(x)):
    print(x[i])
```
Пример 2. Дана строка s = "world". Напечатать все символы строки и их индексы по одному в строке.
```
s = "world"
for i in range(len(s)):
    print(i, s[i])
```
В результате выполнения программы будет выведено:
```
0 w
1 o
2 r
3 l
4 d
```
##### Цикл **for ... in string:**
Синтаксис команды:
```
for <char> in <string>:
    <operator>
```
Здесь `char` - переменная, обозначающая элемент (символ) строки;
`string` - имя строковой переменной; `operator` - одна или несколько команд, которые выполняются в цикле.

Пример 3. Напечатать символы строки s.
```
s = "Python"
for char in s:
    print(char)
```
Пример 4. Посчитать количество цифр в строке poem.
```
poem = "1 potato, 2 potatoes, 3 potatoes, 4!"
count = 0
for el in poem:
    if el.isdigit():
        count += 1
print(count)
```
Пример 5. Ввести имя в строку name. С помощью цикла получить имя в обратном порядке.
```
name = input("Enter your name: ")  # "Alice"
name_reverse = ""
for letter in name:
    name_reverse = letter + name_reverse  # буквы прибавляются по одной справа
print(name_reverse)  # "ecilA"
```
##### Цикл **for ... in enumerate(s)**
Синтаксис команды:
```
for  <index>, <char> in enumerate(<string>):
    <operator>
```
Функция enumerate() используется для упрощения прохода по строке в цикле, когда кроме самих элементов требуется их индекс.
Здесь `index` - переменная, обозначающая индекс элемента строки; `char` - переменная, обозначающая элемент (символ) строки; `string` - имя строки; operator - одна или несколько команд, которые выполняются в цикле.

Пример 6. Ввести имя в строку name. Напечатать все буквы имени и их индексы.
```
name = input("Enter your name: ")
for i, letter in enumerate(name):
    print(f"{i} ---> {letter}")
```

Пример 7. Дана строка. Все символы строки с четными индексами сделать заглавными (uppercase), символы строки с нечетными индексами сделать строчными (lowercase).
```
word = "alternate"
res = ""
for i, letter in enumerate(word):
    if i % 2 == 0:
        res = res + letter.upper()
    else:
        res = res + letter.lower()
print(res)  # "AlTeRnAtE"
```

##### Задания
1.  Ввести строку. Пройти в цикле по строке и вывести индексы символов строки.
1.  Ввести строку. Вывести символы строки и через тире - их индексы. Например, если введена строка "sky", вывести:
```
s - 0
k - 1
y - 2
```
3. Посчитайте количество заглавных букв в строке.
1. Посчитайте общее количество гласных в строке (в верхнем и нижнем регистре).
1. Удвойте все символы строки (путем создания новой строки).
1. Задайте строку с произвольным значением (например, "Python"). Получите строку, в которой все буквы будут разделены пробелами ("P y t h o n").
1. Вставьте пробелы после всех неалфавитных символов строки (путем создания новой строки). Например, s = "Bananas,2apples,sweets and 8plums". Получить "Bananas, 2 apples, sweets  and  8 plums".
1. Задайте строку с произвольным значением (например, "summer"). Получите строку, в которой гласные буквы станут заглавными ("sUmmEr").
1. Дана строка.Замените все гласные буквы на символ "*". При решени задачи используйте цикл и метод replace.
1. Дана строка. Удалите все гласные буквы в строке. При решени задачи используйте цикл и метод replace.
1. Дана строка. Получить две новые строки: одну - из символов с четными индексами, другую - из символов с нечетными индексами. Напримре, s = "separate". Новые строки: "sprt", "eaae".
1. Ввести строку, включающую строчные и прописные буквы. Вывести ту же строку в одном регистре, который зависит от того, каких букв больше. При равном количестве преобразовать в нижний регистр. Например, вводится строка "HeLLo World", она должна быть преобразована в "hello world", потому что в исходной строке малых букв больше. 


