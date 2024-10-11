---
## Front matter
title: "отчёт по лабораторной работе №3"
subtitle: "Архитектура компьютеров НММбд-03-24"
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

Целью данной работы является изучить идеологию и применение средств контроля версий. При-
обрести практические навыки по работе с системой git.

# Выполнение лабораторной работы

1.1 Настроим github (рис. [-@fig:001]).

![настройка github](image/снимок1.png){#fig:001 width=70%}

1.2 Создём ssh ключ (рис. [-@fig:002]).

![ssh ключ](image/снимок2.png){#fig:002 width=70%}

1.3 Создание рабочего пространства и репозитория и его клонирование(рис. [-@fig:003]).

![рабочее пространство и репозиторий](image/снимок3.png){#fig:003 width=70%}

1.4 Настраиваем каталог курса(рис. [-@fig:004])(рис. [-@fig:005])(рис. [-@fig:006]).

![создаём каталоги](image/снимок4.png){#fig:004 width=70%}

![отправляем файлы на сервер](image/снимок5.png){#fig:005 width=70%}

![отправляем файлы на сервер](image/снимок6.png){#fig:006 width=70%}

1.5 выполнение самостоятельной работы

![добавляем файл с отчётом по лабораторной работе №1](image/снимок9.png){#fig:009 width=70%}
![загружаем файл на github](image/снимок10.png){#fig:010 width=70%}
![добавляем файл с отчётом по лабораторной работе №2 и загружаем на github](image/снимок6.png){#fig:006 width=70%}

# Выводы

Я изучила идеологию и применение средств контроля версий и при-
обрела практические навыки по работе с системой git.

