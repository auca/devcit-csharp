# DEVCIT-CSHARP
Практическая работа №8
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

## Задание №1: "Прототип простого графического редактора"

В этом задание вы должны создать консольную программу, которая эмулирует важные составные элементы векторного
графического редактора.

В первой версии прототипа вы должны создать несколько прямоугольников с произвольными координатами
и размером. После этого, ваша программа должна считывать команды пользователя в цикле:

* present: печатает информацию о всех фигурах
* click: считывает координаты x и y и печатает фигуры, в которые указанная точка мышки попала
* stop: останавливает программу

```
command: present
Rectangle: 10, 10, 100, 100
Rectangle: 400, 400, 100, 100
command: click
x: 100
y: 100
Rectangle: 10, 10, 100, 100
command: click
x: 1000
y: 1000
command: click
x: 450
y: 450
Rectangle: 400, 400, 100, 100
command: stop
```

## Задание №2: "Прототип простого графического редактора"

Добавьте несколько окружностей к предыдущему прототипу. Эта версия должна иметь несвязанный
классы:

* Rectangle
* Circle

Объясните недостатки этой версии.

```
command: click
x: 20
y: 20
Rectangle: 10, 10, 100, 100
command: present
Rectangle: 10, 10, 100, 100
Rectangle: 400, 400, 100, 100
Circle: 500, 10, 100
Circle: 800, 800, 100
command: move
x1: 510
y1: 20
x2: 600
y2: 100
command: present
Rectangle: 10, 10, 100, 100
Rectangle: 400, 400, 100, 100
Circle: 590, 90, 100
Circle: 800, 800, 100
command: stop
```

## Задание №3: "Прототип простого графического редактора"

Улчшите структуру предыдущего прототипа путем введения иерархии классов.

Корнем этой иерархии должен стать абстрактный класс `Shape` с общими свойствами и методами
классов `Rectangle` и `Circle`. Классы `Rectangle` и `Circle` должны стать дочерними
классами класса `Shape`.

## Задание №4: "Простой графический редактор"

Создайте простой редактор векторной графики:

* Редактор может создавать фигуры двух типов: Прямоугольники, Окружности.
* Щелчок левой кнопкой мыши рисует выбранную фигуру.
* Правый клик на фигуре выбирает фигуру и позволяет перетащить ее по форме.
* Клавиша `Delete` удаляет выбранную фигуру.
