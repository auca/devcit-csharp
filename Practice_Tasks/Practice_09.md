# DEVCIT-CSHARP
Практическая работа №9
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

## Задание №1: "Метод Array.Sort и интерфейс IComparable"

Напишите программу для сортировки

* Массив из чисел
* Массив из строк
* Массив из объектов `BigInteger`
* Массива объектов `Rational`

...методом `Array.sort` из библиотеки .Net

Для данных ниже

```C#
int[] integers = {
    8, 2, 6, 5, 1, 9, 3
};

// ...

string[] strings = {
    "Java", "C++", "Kotlin", "C#", "Scala", "C"
};

// ...

BigInteger[] bigIntegers = {
    BigInteger.Parse("3874357438573487"),
    BigInteger.Parse("-587485748753874357438573487"),
    BigInteger.Parse("758437584756847534785983749587439587398457"),
    BigInteger.Parse("938493849839584758475847")
};

// ...

Rational[] rationals = {
    Rational.Parse("5/7"),
    Rational.Parse("1/2"),
    Rational.Parse("7/2"),
    Rational.Parse("1/3")
};

// ...
```

...ваша программа должна вывести следующее

```
Sorting integers
Before:
[8, 2, 6, 5, 1, 9, 3]
After:
[1, 2, 3, 5, 6, 8, 9]

Sorting strings
Before:
[Java, C++, Kotlin, C#, Scala, C]
After:
[C, C#, C++, Java, Kotlin, Scala]

Sorting big integers
Before:
[3874357438573487, -587485748753874357438573487, 758437584756847534785983749587439587398457, 938493849839584758475847]
After:
[-587485748753874357438573487, 3874357438573487, 938493849839584758475847, 758437584756847534785983749587439587398457]

Sorting rationals
Before:
[5/7, 1/2, 7/2, 1/3]
After:
[1/3, 1/2, 5/7, 7/2]
```

## Задание №2: "Метод Array.Sort и интерфейс IComparator"

Напишите программу для сортировки массива объектов класса `Student` (класс нужно создать вам) по следующим полям

* Имя (лексикографически)
* GPA (средняя оценка успеваемости [0..4])
* Год рождения

Используйте класс `Array` для сортировки данных. Создайте класс `Student` с полями из списка выше. Создайте классы `ComparerByName`, `ComparerByGPA` и `ComparerByBirthYear`, реализуя интерфейс `IComparer`.

Для данных ниже

```java
Student[] students = {
    new Student("StudentD", 2.5, 1998),
    new Student("StudentA", 4.0, 2001),
    new Student("StudentB", 3.0, 2001),
    new Student("StudentC", 3.5, 2000)
};

// ...
```

...ваша программа должна вывести следующее

```
Sorting students by name
Before:
[Student{name='StudentD', GPA=2.5, birthYear=1998}, Student{name='StudentA', GPA=4.0, birthYear=2001}, Student{name='StudentB', GPA=3.0, birthYear=2001}, Student{name='StudentC', GPA=3.5, birthYear=2000}]
After:
[Student{name='StudentA', GPA=4.0, birthYear=2001}, Student{name='StudentB', GPA=3.0, birthYear=2001}, Student{name='StudentC', GPA=3.5, birthYear=2000}, Student{name='StudentD', GPA=2.5, birthYear=1998}]

Sorting students by GPA
Before:
[Student{name='StudentA', GPA=4.0, birthYear=2001}, Student{name='StudentB', GPA=3.0, birthYear=2001}, Student{name='StudentC', GPA=3.5, birthYear=2000}, Student{name='StudentD', GPA=2.5, birthYear=1998}]
After:
[Student{name='StudentD', GPA=2.5, birthYear=1998}, Student{name='StudentB', GPA=3.0, birthYear=2001}, Student{name='StudentC', GPA=3.5, birthYear=2000}, Student{name='StudentA', GPA=4.0, birthYear=2001}]

Sorting students by birth year
Before:
[Student{name='StudentD', GPA=2.5, birthYear=1998}, Student{name='StudentB', GPA=3.0, birthYear=2001}, Student{name='StudentC', GPA=3.5, birthYear=2000}, Student{name='StudentA', GPA=4.0, birthYear=2001}]
After:
[Student{name='StudentD', GPA=2.5, birthYear=1998}, Student{name='StudentC', GPA=3.5, birthYear=2000}, Student{name='StudentB', GPA=3.0, birthYear=2001}, Student{name='StudentA', GPA=4.0, birthYear=2001}]
```

## Задание №3: "Свой класс MyArray"

Напишите свой собственный класс `MyArray` с методом `Sort`, используя алгоритм сортировки выбором. Создайте свои реализации интерфейсов `MyIComparable` and `MyIComparer`.

Напишите программу для сортировки:

* Массива любых чисел
* Массива объектов `Student`, сортируя по имени лексикографически
* Массива объектов `Rational`

Для данных ниже

```c#
int[] integers = {
    8, 2, 6, 5, 1, 9, 3
};

// ...

Student[] students = {
    new Student("StudentD", 2.5, 1998),
    new Student("StudentA", 4.0, 2001),
    new Student("StudentB", 3.0, 2001),
    new Student("StudentC", 3.5, 2000)
};

// ...

Rational[] rationals = {
    Rational.Parse("5/7"),
    Rational.Parse("1/2"),
    Rational.Parse("7/2"),
    Rational.Parse("1/3")
};
```

...ваша программа должна вывести следующее

```
Sorting integers
Before:
[8, 2, 6, 5, 1, 9, 3]
After:
[1, 2, 3, 5, 6, 8, 9]

Sorting students by name
Before:
[Student{name='StudentD', GPA=2.5, birthYear=1998}, Student{name='StudentA', GPA=4.0, birthYear=2001}, Student{name='StudentB', GPA=3.0, birthYear=2001}, Student{name='StudentC', GPA=3.5, birthYear=2000}]
After:
[Student{name='StudentA', GPA=4.0, birthYear=2001}, Student{name='StudentB', GPA=3.0, birthYear=2001}, Student{name='StudentC', GPA=3.5, birthYear=2000}, Student{name='StudentD', GPA=2.5, birthYear=1998}]

Sorting rationals
Before:
[5/7, 1/2, 7/2, 1/3]
After:
[1/3, 1/2, 5/7, 7/2]
```