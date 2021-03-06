В Python существует конструкция, которая по своему действию аналогична конструкции if-else, но при этом является выражением. Она называется **тернарный оператор**.

Тернарный оператор — единственный в своем роде оператор, требующий три операнда:
```
<value_if true> if <condition > else <value_if_false>
```
Тернарный оператор — способ превратить простую условную инструкцию в выражение, например, 
```
number if number >= 0 else -number
```
Пример 1. Присвоить переменной `description` значение "Even", если введенное число `number` четное, или "Odd" в противном случае.

*1 способ*: с использованием оператора if else:
```
number = int(input("Enter number: "))
if number % 2 == 0:
    description = "Even"
else:
    description = "Odd"
```
*2 способ*: с использованием тернарного оператора:
```
number = int(input("Enter number: "))
description = "Even" if number % 2 == 0 else "Odd"
```
Пример 2. Если имя равно "Bill", напечатать "Hello boss", иначе напечатать "Hello guest".

*1 способ*: с использованием оператора if else:
```
name = "John"
if name == "Bill":
    print("Hello boss")
else:
    print("Hello guest")
```
*2 способ*: с использованием тернарного оператора:
```
name = "John"
print("Hello boss") if name == "Bill" else print("Hello guest")
```

##### Задания.
1. Дана переменная `t`, хранящая значение температуры человека. Присвоить переменой health значение `"healthy"`, если t < 37, и `"Ill"` в противном случае. Выполните это задание двумя способами:  с использованием оператора if else и с использованием тернарного оператора.
1. Дана переменная `num_of_day`, хранящая номер дня недели. Присвоить переменой `day` значение `Weekend`, если номер дня 6 или 7, и `Work day` в противном случае. Выполните это задание двумя способами:  с использованием оператора if else и с использованием тернарного оператора.
1. Дана переменная `number`, хранящая число.  Напечатать удвоенное число,  если число положительное,  или число с обратным знаком -  в противном случае. Выполните это задание двумя способами:  с использованием оператора if else и с использованием тернарного оператора. Например, если number = 9, напечатать 18. Если number = -8, напечатать 8.
1. Дано число n. Число является "счастливым", если оно делится на 9. Присвойте переменной `is_lucky` значение `"Lucky number"`, если число делится на 9, и  `"Not a lucky number"` в противном случае.