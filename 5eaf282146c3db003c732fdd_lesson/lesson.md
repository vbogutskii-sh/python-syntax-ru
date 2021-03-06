Комментарии очень важны при написании программы. Они описывают то, что происходит внутри программы, так что человеку, смотрящему на исходный код, нетрудно его понять.

С помощью комментария вы можете пояснить фрагмент кода. Перед комментарием надо поставить символ #. Строка комментария не является командой программы и игнорируется при выполнении программы. Также, если вы хотите, чтобы какие-то строки программы не выполнялись, вы можете закомментировать эти строки, поставив  символ хэша `#`  в начале строки. После символа # желательно поставить пробел.

```
# This is a comment    
```
**Комментарии в строке с кодом**
Такой комментарий находится в той же строке, что и инструкция. «Встрочные» комментарии должны отделяться хотя бы двумя пробелами от инструкции. Они должны начинаться с символа # и одного пробела.
```   
print("Hello world")   # print hello
```
**Многострочные комментарии**

Чтобы закомментировать несколько строк программы, надо поставить символ хэша в начало каждой строки. Чтобы это сделать быстрее, надо выделить эти строки и нажать сочетание клавиш `ctrl + /` (для Windows) или `command+/` (для Mac).

```
# This is a long comment
# and it takes up
# several lines
```
Другой способ написания многострочного комментария - использование трех кавычек `'''` или `"""`:
```
"""This is also a
perfect example of
multi-line comments"""
```