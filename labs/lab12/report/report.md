---
## Front matter
title: "Лабораторная работа №12"
subtitle: "Программирование в командном процессоре ОС UNIX. Командные файлы"
author: "Кижваткина Анна Юрьевна"

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

Изучить основы программирования в оболочке ОС UNIX/Linux. Научиться писать небольшие командные файлы.

# Выполнение лабораторной работы


Создаем директорию backup. (рис. [-@fig:001])

![Создание директории](image/1.png){#fig:001 width=70%}

Создаем файл task1.sh. (рис. [-@fig:002])

![Создание файла](image/2.png){#fig:002 width=70%}

Пишем скрипт, который при запуске будет делать резервную копию самого себя (то есть файла, в котором содержится его исходный код) в другую директорию backup в вашем домашнем каталоге. При этом файл должен архивироваться одним из архиваторов на выбор zip, bzip2 или tar. Способ использования команд архивации необходимо узнать, изучив справку.  (рис. [-@fig:003])

![Программа](image/3.png){#fig:003 width=70%}

Предоставляем полный доступ (чтение, запись и выполнение) к файлу или каталогу для всех пользователей. (рис. [-@fig:004])

![Предоставление доступа](image/4.png){#fig:004 width=70%}

Проверяем выполнение программы. (рис. [-@fig:005])

![Запуск программы](image/5.png){#fig:005 width=70%}

Создаем файл task2.sh. (рис. [-@fig:006])

![Создание файла](image/6.png){#fig:006 width=70%}

Предоставляем полный доступ (чтение, запись и выполнение) к файлу или каталогу для всех пользователей. (рис. [-@fig:007])

![Предоставление доступа](image/7.png){#fig:007 width=70%}

Пишем пример командного файла, обрабатывающего любое произвольное число аргументов командной строки, в том числе превышающее десять. Например, скрипт может последовательно распечатывать значения всех переданных аргументов. (рис. [-@fig:008])

![Программа](image/8.png){#fig:008 width=70%}

Проверяем выполнение программы. (рис. [-@fig:009])

![Запуск программы](image/9.png){#fig:009 width=70%}

Создаем файл task3.sh. (рис. [-@fig:010])

![Создание файла](image/10.png){#fig:010 width=70%}

Предоставляем полный доступ (чтение, запись и выполнение) к файлу или каталогу для всех пользователей. (рис. [-@fig:011])

![Предоставление доступа](image/11.png){#fig:011 width=70%}

Пишем командный файл — аналог команды ls (без использования самой этой команды и команды dir). Требуется, чтобы он выдавал информацию о нужном каталоге и выводил информацию о возможностях доступа к файлам этого каталога. (рис. [-@fig:012])

![Программа](image/12.png){#fig:012 width=70%}

Проверяем выполнение программы. (рис. [-@fig:013])

![Запуск программы](image/13.png){#fig:013 width=70%}

Создаем файл task4.sh. (рис. [-@fig:014])

![Создание файла](image/14.png){#fig:014 width=70%}

Предоставляем полный доступ (чтение, запись и выполнение) к файлу или каталогу для всех пользователей. (рис. [-@fig:015])

![Предоставление доступа](image/15.png){#fig:015 width=70%}

Пишем командный файл, который получает в качестве аргумента командной строки формат файла (.txt, .doc, .jpg, .pdf и т.д.) и вычисляет количество таких файлов в указанной директории. Путь к директории также передаётся в виде аргумента командной строки. (рис. [-@fig:016])

![Программа](image/16.png){#fig:016 width=70%}

Проверяем выполнение программы. (рис. [-@fig:017])

![Запуск программы](image/17.png){#fig:017 width=70%}

# Выводы

В ходе данной лабораторной работы мы изучили основы программирования в оболочке ОС UNIX/Linux. Научились писать небольшие командные файлы.
