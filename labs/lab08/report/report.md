---
## Front matter
title: "Лабораторная работа 8"
author: "Ефремова Вера"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Познакомиться с операционной системой Linux. Получить практические навыки рабо-
ты с редактором vi, установленным по умолчанию практически во всех дистрибутивах.

# Задание

1. Создайте каталог с именем ~/work/os/lab06.
2. Перейдите во вновь созданный каталог.
3. Вызовите vi и создайте файл hello.sh
1 vi hello.sh
4. Нажмите клавишу i и вводите следующий текст.
1 #!/bin/bash
2 HELL=Hello
3 function hello {
4 LOCAL HELLO=World
5 echo $HELLO
6 }
7 echo $HELLO
8 hello
5. Нажмите клавишу Esc для перехода в командный режим после завершения ввода
текста.
6. Нажмите : для перехода в режим последней строки и внизу вашего экрана появится
приглашение в виде двоеточия.
7. Нажмите w (записать) и q (выйти), а затем нажмите клавишу Enter для сохранения
вашего текста и завершения работы.
8. Сделайте файл исполняемым
1 chmod +x hello.sh

1. Вызовите vi на редактирование файла
1 vi ~/work/os/lab06/hello.sh
2. Установите курсор в конец слова HELL второй строки.
3. Перейдите в режим вставки и замените на HELLO. Нажмите Esc для возврата в команд-
ный режим.
4. Установите курсор на четвертую строку и сотрите слово LOCAL.
5. Перейдите в режим вставки и наберите следующий текст: local, нажмите Esc для
возврата в командный режим.
6. Установите курсор на последней строке файла. Вставьте после неё строку, содержащую
следующий текст: echo $HELLO.
7. Нажмите Esc для перехода в командный режим.
8. Удалите последнюю строку.
9. Введите команду отмены изменений u для отмены последней команды.
10. Введите символ : для перехода в режим последней строки. Запишите произведённые
изменения и выйдите из v

# Выполнение лабораторной работы

1. Создали каталог с именем ~/work/os/lab06.Перешли во вновь созданный каталог.Вызвали vi и создали файл hello.sh(рис. @fig:001).

![Создание и переход](image/1.jpg){#fig:001 width=70%}

2. Нажали клавишу i и ввели текст из задания. Перешли в командный режим и ввели для записи и выхода :wq, а потом enter для сохранения (рис. @fig:002) 

![Ввод текста](image/2.jpg){#fig:002 width=70%}

3. Потом мы сделали файл исполняемым и вызвали на редактирование(рис. @fig:003)

![редактирование](image/3.jpg){#fig:003 width=70%}

4. С помощью стрелок установили курсор в конец слова HELL второй строки. Перешли в режим вставки i и заменили на HELLO. Нажали на Esc для возврата в командный режим. (рис. @fig:004)

![изменение 1](image/4.jpg){#fig:004 width=70%}

5. Установили курсор на четвертую строку и стерли слово LOCAL. Перешли в режим вставки и набрали local, нажали Esc для
возврата в командный режим.(рис. @fig:005)

![замена](image/5.jpg){#fig:005 width=70%}

6. Установили курсор на последней строке файла. Вставили после неё строку, содержащую
следующий текст: echo $HELLO, предварительно скопировав данный текст с другой строки.(рис. @fig:006)

![копирование](image/6.jpg){#fig:006 width=70%}

7. Удалили последнюю строку с помощью dd .Ввели команду отмены изменений u для отмены последней команды. Ввели символ : для перехода в режим последней строки. Записали произведённые изменения с помощью wq и вышли.  (рис. @fig:007)

![сохраение](image/7.jpg){#fig:007 width=70%}

# Выводы

Познакомились с операционной системой Linux. Получили практические навыки рабо-
ты с редактором vi, установленным по умолчанию практически во всех дистрибутивах.

::: {#refs}
:::
