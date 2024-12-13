---
## Front matter
title: "Отчёт по лабораторной работе №8"
subtitle: "Архитектура компьютера НММбд 03-24"
author: "Топорова Дарья Сергеевна"

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
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
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

Целбю работы является приобретение навыков написания программ с использованием циклов и обработкой
аргументов командной строки в NASM.

# Задание

1. Напишите программу, которая находит сумму значений функции f(x) для x = x1, x2, …, xn, т.е. программа должна выводить значение f(x1) + f(x2) + … + f(xn). Значения xi передаются как аргументы. Вид функции f(x) выбрать из таблицы 8.1 вариантов заданий в соответствии с вариантом, полученным при выполнении лабораторной работы № 7. Создайте исполняемый файл и проверьте его работу на нескольких наборах x = x1, x2 …, xn.

# Выполнение лабораторной работы

1.1 создаю каталог lab08 и файл для выполнения лабораторную №8

![создаём каталог и файл](image/screen.jpg){#fig:001 width=60%}

1.2 Ввожу в файл lab8-1.asm программу вывода значени региста eax из листинга 8.1. Запускаю исполняемый файл.

![Программа вывода значений регистра ecx](image/screen1.jpg){#fig:002 width=60%}
![результат программы из lab8-1.asm](image/screen7.jpg){#fig:003 width=60%}

1.3 Изменим текст программы, добавив изменение значение регистра ecx в цикле. Запускаем изменённую программу. Теперь число проходов цикла не соответствует значению, введённому с клавиатуры.

![Изменённый текст программы lab8-1.asm](image/screen3.5.jpg){#fig:004 width=60%}
![результат выполнения программы](image/screen2.jpg){#fig:005 width=60%}

1.4 Внесём изменения в текст программы добавив команды push и pop для сохранения значения счетчика цикла loop. Запускаем программу и проверим ее работу. Число проходов цикла соответствует числу, введённому с клавиатуры.

![Изменённый текст программы lab8-1.asm с помощью pop и push](image/screen4.jpg){#fig:006 width=60%}
![результат выполнения программы](image/screen3.jpg){#fig:007 width=60%}

2.1 создаём файл lab8-2.asm. Вводим программу выводящую на экран аргументы командной строки из листинга 8.2. Запускаю исполняемый файл.

![программа выводящая на экран аргументы командной строки](image/screen6.jpg){#fig:008 width=60%}
![результат выполнения программы из файла lab8-2.asm](image/screen5.jpg){#fig:009 width=60%}

2.2 создаём файл lab8-3.asm. Введём программу по вычислению суммы аргументов командной строки, запустим исполняемый файл.

 ![Программа вычисления суммы аргументов командной строки](image/screen9.jpg){#fig:010 width=60%}
 ![результат выполнения программы из файла lab8-3.asm](image/screen8.jpg){#fig:011 width=60%}

2.3 Изменяем текст программы из листинга 8.3 для вычисления произведения аргументов
командной строки.

 ![Программа для вычисления произведения аргументов командной строки.](image/screen10.jpg){#fig:012 width=60%}
 ![результат выполнения программы из файла lab8-3.asm](image/screen11.jpg){#fig:013 width=60%}

# Выполнение самостоятельной работы

3.1 Напишем программу, которая находит сумму значений функции f(x) для x=x1, x2, …, xn, т.е. программа должна выводить значение f(x1) + f(x2) + … + f(xn). Мой вариант - 16. Создадим исполняемый файл и проверим его работу на нескольких наборах x=x1, x2, …, xn. 

 ![Программа lab8-4.asm](image/screen13.jpg){#fig:014 width=60%}
 ![Результат программы](image/screen12.jpg){#fig:015 width=60%}

# Выводы

В результате выполнения лабораторной работы я приобрёл навыки написания программ с использованием циклов и обработкой аргументов командной строки в NASM.
