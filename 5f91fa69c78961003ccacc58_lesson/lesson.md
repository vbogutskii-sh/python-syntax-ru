Чтобы проверить наличие элемента с заданным ключом в словаре, используют оператор **in**. Если ключ есть в словаре, получим значение True, в противном случае – False. 

**Пример 1**. Есть словарь с именем user. Проверить, если ли в словаре ключи "age" и "address".
```
user = {
  "name": "Alice",
  "age": 30,
  "is_Student": True,
}
print("age" in user)  # True
print("address" in user)  # False
```
**Пример 2**. Проверить, есть ли в словаре mountains гора Арарат высотой 5165 м.
```
mountains = {
  4810: "Mont Blanc",
  8848: "Mount Everest",
  4317: "Mount Shasta",
  5881: "Kilimanjaro"
 }
print(5165 in mountains) #  False
```
##### Задания
1. Словарь хранит информацию о запасах фруктов на складе. Определите, есть ли на складе апельсины ("orange")
```
fruits = { 
  'apple': 40, 
  'orange': 25, 
  'mango': 50
}
```
2. Словарь хранит информацию о кинофильме. Определите, хранит ли словарь информацию о годе создания фильма ('year').
```
movie = {
  'name': 'Groundhog day',
  'type': 'comedy',
  'year': 1993,
}
```


3. Словарь хранит информацию об отметках студента. Определите, хранит ли словарь информацию об успеваемости по математике ('math').
```
report = {
  'math': 5,
  'history': 4,
  'science': 5,
}
```
