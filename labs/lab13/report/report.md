---
## Front matter
title: "Лабораторная работа №13"
subtitle: "Программирование в командном процессоре ОС UNIX. Ветвления и циклы"
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

Изучить основы программирования в оболочке ОС UNIX. Научится писать более сложные командные файлы с использованием логических управляющих конструкций и циклов.

# Выполнение лабораторной работы

Создаем директорию lab13 и перемещаемся в неё. (рис. [-@fig:001])

![Создание директории](image/1.png){#fig:001 width=70%}

Создаем файл 1.sh и text. (рис. [-@fig:002])

![Создание файла](image/2.png){#fig:002 width=70%}

Используя команды getopts grep, написать командный файл, который анализирует командную строку с ключами: 

	– -iinputfile — прочитать данные из указанного файла; 
	– -ooutputfile — вывести данные в указанный файл; 
	– -pшаблон — указать шаблон для поиска; 
	– -C — различать большие и малые буквы; 
	– -n — выдавать номера строк. 
	
а затем ищет в указанном файле нужные строки, определяемые ключом -p. (рис. [-@fig:003])

![Программа](image/3.png){#fig:003 width=70%}

Устанавливаем право на выполнение. (рис. [-@fig:004])

![Предоставление доступа](image/4.png){#fig:004 width=70%}

Проверяем выполнение программы. (рис. [-@fig:005])

![Запуск программы](image/5.png){#fig:005 width=70%}

Создаем файл 2.sh и 2.с и устанавливаем право на выполнение. (рис. [-@fig:006])

![Создание файла](image/6.png){#fig:006 width=70%}

Написать на языке Си программу, которая вводит число и определяет, является ли оно больше нуля, меньше нуля или равно нулю. Затем программа завершается с помощью функции exit(n), передавая информацию в о коде завершения в оболочку. Командный файл должен вызывать эту программу и, проанализировав с помощью команды $?, выдать сообщение о том, какое число было введено. (рис. [-@fig:007] и рис. [-@fig:008])

![Программа](image/7.png){#fig:007 width=70%}

![Программа](image/8.png){#fig:008 width=70%}

Проверяем выполнение программы. (рис. [-@fig:009])

![Запуск программы](image/9.png){#fig:009 width=70%}

Создаем файл 3.sh. (рис. [-@fig:010])

![Создание файла](image/10.png){#fig:010 width=70%}

Устанавливаем право на выполнение. (рис. [-@fig:011])

![Предоставление доступа](image/11.png){#fig:011 width=70%}

Написать командный файл, создающий указанное число файлов, пронумерованных последовательно от 1 до 𝑁 (например 1.tmp, 2.tmp, 3.tmp, 4.tmp и т.д.). Число файлов, которые необходимо создать, передаётся в аргументы командной строки. Этот же командный файл должен уметь удалять все созданные им файлы (если они существуют). (рис. [-@fig:012])

![Программа](image/12.png){#fig:012 width=70%}

Проверяем выполнение программы. (рис. [-@fig:013])

![Запуск программы](image/13.png){#fig:013 width=70%}

Создаем файл 4.sh. (рис. [-@fig:014])

![Создание файла](image/14.png){#fig:014 width=70%}

Устанавливаем право на выполнение. (рис. [-@fig:015])

![Предоставление доступа](image/15.png){#fig:015 width=70%}

Написать командный файл, который с помощью команды tar запаковывает в архив все файлы в указанной директории. Модифицировать его так, чтобы запаковывались только те файлы, которые были изменены менее недели тому назад (использовать команду find). (рис. [-@fig:016])

![Программа](image/16.png){#fig:016 width=70%}

Проверяем выполнение программы. (рис. [-@fig:017] и рис. [-@fig:018])

![Запуск программы](image/17.png){#fig:017 width=70%}

![Запуск программы](image/18.png){#fig:018 width=70%}

# Выводы

С помощью данной лабораторной работы мы изучили основы программирования в оболочке ОС UNIX. Научились писать более сложные командные файлы с использованием логических управляющих конструкций и циклов.
