# DEVCIT-CSHARP
Практическая работа №3
======================

## Организация работ

Рекомендуется выделить отдельную директорию для всех практических работ и задач.

### Пример организации директории

```
...
|
|--devcit-csharp
|----practice-01-task-01
|----practice-01-task-02
|----...
|----practice-01-hometask-01
|----practice-01-hometask-02
|----...
|----practice-02-task-01
|----practice-02-task-02
|----...
|----uri-1001
|----uri-1002
|----...
```

## Ключевые инструменты разработчика

* [Visual Studio Code](https://code.visualstudio.com)

### Альтернативные среды разработки (по желанию)

* [Visual Studio](https://visualstudio.microsoft.com)
* [IntelliJ Rider](https://www.jetbrains.com/rider)

## Задание №1: Абсолютное значение

Программа запрашивает одно вещественное число у пользователя (положительное или
отрицательное) и выводит его абсолютное значение.

### Примеры ввода и вывода

```
Введите вещественное число: -123.345
|-123.345| = 123.345
```

```
Введите вещественное число: 12.4
|12.4| = 12.4
```

## Задание №2: Четные и нечетные числа

Программа считывает целое число у пользователя и сообщает является ли оно
четным или нечетным.

### Примеры ввода и вывода

```
Введите число: 2
Число 2 является четным.
```

```
Введите число: 1
Число 1 является нечетным.
```

## Задание №3: Сравнение двух чисел

Программа считывает два целых значения у пользователя и выводит результат
сравнения в следующей форме:

### Примеры ввода и вывода

```
Введите первое число: 123
Введите второе число: 56
Первое число 123 больше второго числа 56.
```

```
Введите первое число: 423
Введите второе число: 1122
Второе число 1122 больше первого числа 423.
```

```
Введите первое число: 42
Введите второе число: 42
Числа равны.
```

## Задание №4: Максимальное из трёх чисел

Программа считывает три целых значения у пользователя и находит максимальное из
них.

### Примеры ввода и вывода

```
Введите первое число: 12
Введите второе число: 7
Введите третье число: 539
Значение 539 является максимальным.
```

```
Введите первое число: 74
Введите второе число: 23
Введите третье число: 23
Значение 74 является максимальным.
```

## Задание №5: Опасное сравнение №1

Создайте переменную типа `double` равную `0`. Сложите 10 раз значение переменной
с фиксированным значением `0.1`. Сравните финальное значение с `1.0`. Если
значенияравны, выведите сообщение "Равны", иначе "Не равны". Запустите программу
и объясните результат. Покажите корректный способ сравнения для чисел с
плавающей запятой.

## Задание №6: Опасное сравнение №2

Создайте переменную типа `double` равную `9007199254740992`. Сравните финальное
значение с числом `9007199254740993`. Если значения равны, выведите сообщение
"Равны", иначе "Не равны". Запустите программу, объясните результат.

## Задание №7: Високосный год

Напишите программу, которая сообщает, является ли введённый год високосным.

### Тестовые данные

#### Високосные года

1796, 1804, 1896, 1904, 1992, 1996, 2000, 2004, 2008

#### Невисокосные года

1799, 1800, 1801, 1802, 1803, 1805, 1899, 1900, 1901

### Примеры ввода и вывода

```
Введите год: 2000
2000 является високосным годом.
```

```
Введите год: 1800
1800 НЕ является високосным годом.
```

## Задание №8: Оценки

Напишите программу, которая по заданной числовой оценке найдёт буквенную оценку.

### Таблица перевода

```
90 <= A <= 100
80 <= B < 90
70 <= C < 80
60 <= D < 70
Меньше 60: F
```

### Примеры ввода и вывода

```
Введите количество баллов: 73
Оценка: C
```

```
Введите количество баллов: 120
Значение 120 является некоректным
```

## Задание №9: Название месяца (if-else if)

Напишите программу, которая по заданному номеру месяца выводит его название. В
этом задание вы должны использовать конструкцию `if`.

### Примеры ввода и вывода

```
Введите номер месяца: 12
Декабрь
```

```
Введите номер месяца: 1
Январь
```

```
Введите номер месяца: -10
Неверный номер месяца
```

## Задание №10: Название месяца (switch)

Измените конструкцию `if` решение задания №9 на конструкцию `switch`.

## Задание №11: Название сезона (if-else if)

Напишите приложение для определения названия сезона по номеру месяца. В этом
задание вы должны использовать конструкцию `if`.

### Примеры ввода и вывода

```
Введите номер месяца: 12
Зима
```

```
Введите номер месяца: 3
Весна
```

```
Введите номер месяца: 42
Неверный номер месяца
```

## Задание №12: Название сезона (switch)

Измените конструкцию `if` решение задания №11 на конструкцию `switch`.

## Задание №13: Количество дней

Напишите программу, которая может по заданному году и месяцу определить
количество дней в месяце.

### Примеры ввода и вывода

```
Введите год: 2000
Введите номер месяца: 2
29
```

```
Введите год: 1900
Введите номер месяца: 2
28
```

```
Введите год: 2004
Введите номер месяца: 4
30
```

## Домашнее задание №1: ОРТ

Напишите программу, которая спрашивает в каком классе учится ученик. Если класс
больше 10-го, то программа должна вывести сообщение, что нужно готовиться к ОРТ (Общереспубликанскому Тестированию). Программа не должна ничего выводит во всех
остальных случаях.

```
В каком классе вы учитесь: 10
Нужно готовиться к ОРТ.
```

```
В каком классе вы учитесь: 5
```

## Домашнее задание №2: Точка внутри прямоугольника

Напишите программу, которая предложит ввести точку (x, y) и проверит,
находится ли она в пределах прямоугольника в координатах (0, 0) с шириной 10
и высотой 5. Координата (0, 0) – это центр прямоугольника.

### Примеры ввода и вывода

```
Введите координаты точки (x, y): 2 2
Точка (2.0, 2.0) внутри прямоугольника
```

```
Введите координаты точки (x, y): 6 4
Точка (6.0, 4.0) НЕ внутри прямоугольника
```

## Домашнее задание №3: Точка внутри окружности

Напишите программу, которая предложит ввести точку (x, y) и проверит,
находится ли она в пределах окружности в координатах (10, -5) с радиусом 8.
Координата (10, -5) – это центр окружности.

### Примеры ввода и вывода

```
Введите координаты точки (x, y): 10 -6
Точка (10.0, -6.0) внутри окружности
```

```
Введите координаты точки (x, y): 17 2
Точка (17.0, 2.0) НЕ внутри окружности
```

## Домашнее задание №4: Цена доставки

Компания Evergreen определяет цену доставки груза морским сообщением в Роттердам
исходя из следующей тарифной сетки

```
цена(вес) =
    3.5  тыс. USD: если 0    < вес <= 100 кг.
    5.5  тыс. USD: если 100  < вес <= 300 кг.
    8.5  тыс. USD: если 300  < вес <= 1000 кг.
    10.5 тыс. USD: если 1000 < вес <= 2000 кг.
```

Напишите программу, которая предложит пользователю ввести вес груза и отобразит
стоимость доставки. Если вес больше 2000 кг., то программа должна вывести
сообщение: "Груз не может быть отправлен".

### Пример ввода и вывода

```
Введите вес груза: 150
Цена доставка: 5500 USD
```

## Домашнее задание №5: Карты

Напишите программу, имитирующую выбор карты из колоды из 52-х карт. Ваша
программа должна выбрать ранг (Туз, 2, 3, 4, 5, 6, 7, 8, 9, 10, Валет, Королева,
Король) и масть (Трефы, Бубны, Червы, Пики) карты. Используйте `Math.random()`
вместе с условными конструкциями для решения этой задачи.

### Примеры ввода и вывода

```
Карта, которую вы выбрали — это "Валет червей".
```

### URI

Задания с 1035–1038, 1040–1052, 1061 <https://www.urionlinejudge.com.br/judge/en/problems/index/1>

Перевод заданий можно найти по ссылке

* <https://github.com/auca/devcit-js/blob/master/Practice/URI_Translations_Part_3.md>
* <https://github.com/auca/devcit-js/blob/master/Practice/URI_Translations_Part_4.md>
