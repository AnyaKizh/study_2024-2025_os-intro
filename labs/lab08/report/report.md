---
## Front matter
title: "Oтчёт по лабораторной работе 8"
subtitle: "Поиск файлов. Перенаправление ввода-вывода. Просмотр запущенных процессов"
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

Ознакомление с инструментами поиска файлов и фильтрации текстовых данных. Приобретение практических навыков: по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем.

# Выполнение лабораторной работы

Осуществляем вход в систему, используя соответствующее имя пользователя. Запишем в файл file.txt названия файлов, содержащихся в каталоге /etc. (рис. [-@fig:001])

![Запись названий файлов в файл](image/1.png){#fig:001 width=70%}

Дописываем в этот же файл названия файлов, содержащихся в нашем домашнем каталоге. (рис. [-@fig:002])

![Запись названий файлов в файл](image/2.png){#fig:002 width=70%}

Выводим имена всех файлов из file.txt, имеющих расширение .conf. (рис. [-@fig:003])

![Вывод имен файлов](image/3.png){#fig:003 width=70%}

Записываем их имена в новый файл conf.txt. (рис. [-@fig:004])

![Запись имен в файл](image/4.png){#fig:004 width=70%}

Определяем какие файлы в домашнем каталоге имеют имена, начинающиеся с символа с. (рис. [-@fig:005] рис. [-@fig:006])

![Вывод имен файлов на с](image/5.png){#fig:005 width=70%}
![Вывод имен файлов на с](image/6.png){#fig:006 width=70%}

Выводим имена всех файлов из каталога /etc, начинающиеся с h. (рис. [-@fig:007])

![Вывод файлов на h](image/7.png){#fig:007 width=70%}

Запускаем в фоновом режиме процесс, который будет записывать в файл ~/logfile файлы, имена которых начинаются с log. (рис. [-@fig:008])

![Запуск фонового процесса](image/8.png){#fig:008 width=70%}

Запускаем из консоли в фоновом режиме gedit. (рис. [-@fig:009])

![Запуск фонового процесса gedit](image/9.png){#fig:009 width=70%}

Определяем идентификатор процесса. (рис. [-@fig:010] рис. [-@fig:011] рис. [-@fig:012])

![Определение идентификатора](image/10.png){#fig:010 width=70%}
![Определение идентификатора](image/11.png){#fig:011 width=70%}
![Определение идентификатора](image/12.png){#fig:012 width=70%}

Читаем справку о kill. (рис. [-@fig:013])

![Справка о kill](image/13.png){#fig:013 width=70%}

Завершаем gedit командой kill. (рис. [-@fig:014]) 

![Завершение фонового процесса](image/14.png){#fig:014 width=70%}

Читаем справку о df и du. (рис. [-@fig:015] рис. [-@fig:016])

![команда df](image/15.png){#fig:015 width=70%}
![Команда du](image/16.png){#fig:016 width=70%}

Запускаем df и du. (рис. [-@fig:017] рис. [-@fig:018])

![команда df](image/17.png){#fig:017 width=70%}
![Команда du](image/18.png){#fig:018 width=70%}

Командой find выводим имена всех директорий из домашнего каталога. (рис. [-@fig:019])

![Вывод имен директорий](image/19.png){#fig:019 width=70%}


# Выводы

Мы ознакомились с инструментами поиска файлов и фильтрации текстовых данных. Приобрели практические навыки: по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем.
