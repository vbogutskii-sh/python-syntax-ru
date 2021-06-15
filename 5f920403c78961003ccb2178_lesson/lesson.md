Перебор всех элементов словаря можно сделать с помощью цикла for.  

**Пример 1**. Получим перечень всех ключей словаря mountains и сохраним в виде списка в переменной mount_keys.
```
timetable = {
  8.10: 'morning exercise',
  9.15: 'breakfast',
  9.45: 'college',
 15.30: 'lunch'
}
for event in timetable:
	print(event, ':', timetable[event])  # 8.1 : morning exercise
                                           9.15 : breakfast
                                           9.45 : college
                                           15.3 : lunch
```
Как мы видим, на каждом шаге цикла переменной event присваивают ключ очередного элемента из словаря timetable. Цикл будет работать, пока не переберёт все элементы словаря.

##### Задания
1. Создайте словарь, описывающий автомобиль. Напечатайте перечень всех элементов словаря, пройдя по нему циклом for.
