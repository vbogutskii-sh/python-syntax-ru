* **rjust()** - выравнивание по правому краю. Возвращает строку `str`, выровненную по правому краю в строке длиной `width`. Заполнение выполняется с помощью указанного символа `fillchar` (по умолчанию используется символ пробела). Если width меньше или равен len(str), то возвращается исходная строка.
```
str.rjust(width[, fillchar])
```

* **ljust()** - выравнивание по левому краю. Возвращает строку `str`, выровненную по левому краю в строке длиной `width`. Заполнение выполняется с помощью указанного символа `fillchar` (по умолчанию используется символ пробела). Если width меньше или равен len(str), то возвращается исходная строка.
```
str.rjust(width[, fillchar])
```

* **center()** - выравнивание по центру. Возвращает строку `str`, выровненную по центру строки длиной `width`. Заполнение выполняется с помощью указанного символа `fillchar` (по умолчанию используется символ пробела). Если width меньше или равен len(str), то возвращается исходная строка.
```
str.center(width[, fillchar])
```


Пример 1. Расположить слова по  левому краю, по правому краю, по центру строки длиной 20.
```
word = "left"
print(word.ljust(20))   #  "left                "
word = "right"
print(word.center(20))  #  "               right"
word = "center"
print(word.center(20))  #  "       center       "       
```
##### Задания
1. С помощью функции input введите `first_name`, `middle_name`, `last_name`. Выведите эти три слова в столбик, выравнивание по правому краю. Используйте функцию max для нахождения максимальной длины слов.
```
      Ava
Charlotte
    Smith
```
2. С помощью функции input введите слово word. Введите ширину рамки width. Напечатайте слово в центре рамки шириной width. Если слово невозможно поместить в рамку этой ширины, напечатайте "Error". 
```
********************
*      python      *
********************
```