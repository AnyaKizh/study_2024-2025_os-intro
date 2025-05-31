---
## Front matter
title: "Индивидуальный проект"
subtitle: "Этап №6"
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

Целью данного этапа является сделать английскую версию сайта, чтобы можно было переключаться между языками.

# Задание

	1. Создать отдельные папки для русского и английского 
	2. Перевести все посты и всю информацию
	3. Залить изменения на сайт

# Выполнение лабораторной работы

Создаем директорию ru и en. (рис. [-@fig:001])

![Создание директории](image/1.png){#fig:001 width=70%}

Копируем файлы из папки content в папки ru и en. В ru будут посты на русском, а в en соответственно на английском. (рис. [-@fig:002])

![Перенос файлов](image/2.png){#fig:002 width=70%}

Скачиваем файлы для перевода из репозитория hugo. (рис. [-@fig:003])

![Файлы перевода](image/3.png){#fig:003 width=70%}

Переносим в en нужный файл. (рис. [-@fig:004])

![файлы](image/4.png){#fig:004 width=70%}

Переносим в ru нужный файл. (рис. [-@fig:005])

![файлы](image/5.png){#fig:005 width=70%}

Переписываем файл с языками. (рис. [-@fig:006])

![Код](image/6.png){#fig:006 width=70%}

После запуска сервера появится кнопка смены языка. (рис. [-@fig:007] )

![Кнопка](image/7.png){#fig:007 width=70%}

Переводим файл про автора сайта и перезапускаем сайт, теперь описание можно прочитать на английском. (рис. [-@fig:008])

![Описание на английском](image/8.png){#fig:008 width=70%}

Переводим все предыдущие посты на английский. (рис. [-@fig:009])

![Перевод](image/9.png){#fig:009 width=70%}

Пишем пост про прошедшую неделю на двух языках. (рис. [-@fig:010])

![Пост](image/10.png){#fig:010 width=70%}

Заливаем изменения в github, перезапускаем сайт и видим что изменения применились. (рис. [-@fig:011])

![Запуск сайта](image/11.png){#fig:011 width=70%}

# Выводы

Я сделала возможность переводить сайт с русского на английский, перевела все посты, сделала новые и применила изменения.
