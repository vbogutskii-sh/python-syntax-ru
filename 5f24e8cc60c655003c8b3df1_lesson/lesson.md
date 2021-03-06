Иногда нам надо повторять один и тот же набор действий во многих частях программы. Чтобы не повторять один и тот же код во многих местах, придуманы функции. 

Чтобы создать функцию в Python, нужно указать служебное слово `def`,  после него имя функции, затем cписок параметров в круглых скобках через запятую, затем символ двоеточие. В новой строке с отступом записывается последовательность команд функции, которые также называются телом функции.

Синтаксис функции:
```
def <имя функции>(параметры):
    тело функции
```
Функция после выполнения должна возвращать какое-либо значение. Для того, чтобы возвратить значение, используется оператор `return`. Директива `return` может находиться в любом месте тела функции. Как только выполнение доходит до этого места, функция останавливается, и значение возвращается в вызвавший её код.

Пример.  Функция для вычисления суммы двух чисел.
```
def add(a, b):
    return  a + b

print(add(4, 8))  #  вызов функции add c параметрами 4 и 8,  будет напечатано 12

x = 19
y = 23
s = add(x, y)
print(s)  # 42
```
Функция может не возвращать никаких значений, например,
```
def say_hello():
    print("Hello!")


say_hello()   # будет напечатано слово "Hello!"
say_hello()   #  и еще раз будет напечатано "Hello!"
```
Если в функции отсутствует return, то функция возвращает значение  `None`.

##### Задания
1. Напишите функцию с именем `greet`, которая возвращает фразу "Hello world!" 
1. Напишите функцию с именем `hello_user`, которая принимает имя name в качестве параметра и возвращает фразу "Hello name" (вместо name должно быть имя, переданное в функцию в качестве параметра).
1. Напишите функцию с именем `say_hello`, которая принимает два строковых параметра (name и time). Time может быть "morning", "afternoon", "evening" или "night". Функция должна возвращать приветствие пользователя по имени в зависимости от времени суток: "Good" + time + name (например, "Good evening Samanta!"
1. Напишите функцию с именем `product`, которая принимает три параметра (числа) и возвращает их произведение.
1. Напишите функцию с именем `opposite`, которая принимает число и возвращает противоположное по значению число.
1. Напишите функцию `distance_from_origin`, которая принимает два числа x,y (координаты точки на плоскости)
и возвращает расстояние от этой точки до начала координат. 
1. Напишите функцию `distance`, которая принимает четыре аргумента: x1, y1 (координаты первой точки на плоскости) и x2, y2 (координаты второй точки на плоскости) и возвращает расстояние между точками. Расстояние между точками (x1, y1) и (x2, y2) равно `((x2 - x1)**2 + (y2 - y1)**2) ** 0.5`.
1. Напишите функцию `percentage`, которая принимает два аргумента: `number` и `percent`
и возвращает процент от числа.
1. Индекс массы тела рассчитывается путем деления массы тела (в килограммах) на квадрат роста (в метрах квадратных). Напишите функцию `body_mass_index`, которая принимает два аргумента: `weight` и `height` и возвращает индекс массы тела.
1. Напишите функцию `average`, которая принимает два числа: `a` и `b` и возвращает среднее арифметическое этих чисел.
 1. Напишите функцию `geometric_mean`, которая принимает два числа: `num1` и `num2` и возвращает среднее геометрическое этих чисел. Чтобы найти среднее геометрическое двух чисел, нужно перемножить эти числа и извлечь из них корень. 
1. Сумма углов n-угольника равна 180 * (n − 2).Напишите функцию `angles_of_polygon`, которая принимает аргумент `n` (число углов) и возвращает сумму углов n-угольника.
1. Напишите функцию с именем `miles_to_feet`, которая принимает число `miles` (количество миль)
в качестве аргумента и возвращает это расстояние в футах.
1 миля = 5280 футов.
1. Напишите функцию с именем `centigrade`, которая принимает значение температуры в градусах Фаренгейта `tempF` в качестве аргумента и возвращает значение температуры в градусах Цельсия.

![temperature](https://github.com/bogutski/jsp/blob/master/section-2/temperature.png?raw=true)

15. Напишите функцию с именем `fahrenheit`, которая принимает значение температуры в градусах Цельсия `tempС` в качестве аргумента и возвращает значение температуры в градусах Фаренгейта.

![temperature](https://github.com/bogutski/jsp/blob/master/section-2/farengeitFromCelsium.png?raw=true)