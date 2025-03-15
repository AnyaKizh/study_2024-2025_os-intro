---
## Front matter
title: "Oтчёт по лабораторной работе 5"
subtitle: "Операционные системы"
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

Целью данной лабораторной работы является создание рабочего пространства для дальнейшего использования.

# Выполнение лабораторной работы

Установим pass. (рис. [-@fig:001])

![Установка pass](image/1.png){#fig:001 width=70%}

Установим gopass. (рис. [-@fig:002])

![Установка gopass](image/2.png){#fig:002 width=70%}

Просмотрим список ключей. (рис. [-@fig:003])

![Проверка списка ключей](image/3.png){#fig:003 width=70%}

Инициализируем хранилище при помощи почты. (рис. [-@fig:004])

![Инициализация хранилища](image/4.png){#fig:004 width=70%}

Переходим к синхронизации с git. Создаем структуру git. (рис. [-@fig:005])

![Создание структуры](image/5.png){#fig:005 width=70%}

Предварительно создав репозиторий, задаем адрес репозитория на хостинге. (рис. [-@fig:006])

![Задаем адрес репозитория](image/6.png){#fig:006 width=70%}

Выполняем синхронизацию двумя командами. (рис 2.7. и рис. 2.8.)(рис. [-@fig:007] рис. [-@fig:008])

![Синхронизация](image/7.png){#fig:007 width=70%}

![Синхронизация](image/8.png){#fig:008 width=70%}

Коммитим вручную. Переходим в нужный каталог. (рис. [-@fig:009])

![Перемещение](image/9.png){#fig:009 width=70%}

Выкладываем изменения. (рис. [-@fig:010])

![Выкладывание изменений](image/10.png){#fig:010 width=70%}

Проверяем статус синхронизации командой. (рис. [-@fig:011])

![Проверка синхронизации](image/11.png){#fig:011 width=70%}

Скачиваем плагин для firefox. (рис. [-@fig:012])

![Плагин](image/12.png){#fig:012 width=70%}

Скачиваем интерфейс для взаимодействия с броузером. (рис. [-@fig:013] рис. [-@fig:014])

![Скачивание интерфейса](image/13.png){#fig:013 width=70%}

![Скачивание интерфейса](image/14.png){#fig:014 width=70%}

Создаем файл для пароля. (рис. [-@fig:015])

![Создание файла](image/15.png){#fig:015 width=70%}

Добавляем новый пароль. (рис. [-@fig:016])

![Добавление пароля](image/16.png){#fig:016 width=70%}

Отобразим пароль для указанного имени файла. (рис. [-@fig:017])

![Отображение пароля](image/17.png){#fig:017 width=70%}

Заменим существующий пароль новым. (рис. [-@fig:018])

![Замена пароля](image/18.png){#fig:018 width=70%}

Установим дополнительное программное обеспечение. (рис. [-@fig:019])

![Установка программного обеспечения](image/19.png){#fig:019 width=70%}

Установим шрифты. (рис. [-@fig:020] рис. [-@fig:021] рис. [-@fig:022])

![Установка шрифтов](image/20.png){#fig:020 width=70%}

![Установка шрифтов](image/21.png){#fig:021 width=70%}

![Установка шрифтов](image/22.png){#fig:022 width=70%}

Устанавливаем бинарный файл. (рис. [-@fig:023])

![Установка бинарного файла](image/23.png){#fig:023 width=70%}

Создадим новый репозиторий для конфигурационных файлов на основе шаблона. (рис. [-@fig:024])

![Создание репозитория](image/24.png){#fig:024 width=70%}

Инициализируем chezmoi с нашим репозиторием dotfiles. (рис. [-@fig:025])

![Инициализация](image/25.png){#fig:025 width=70%}

Проверим какие изменения внесет chezmoi в домашний каталог. (рис. [-@fig:026])

![Проверка](image/26.png){#fig:026 width=70%}

Проверяем устраивают ли нас изменения, дальше принимаем их. (рис. [-@fig:027])

![Принятие изменений](image/27.png){#fig:027 width=70%}

Открываем вторую виртуальную машину. Инициализируем на ней chezmoi с репозиторием dotfiles. (рис. [-@fig:028])

![Инициализация](image/28.png){#fig:028 width=70%}

Проверим какие изменения внесет chezmoi. (рис. [-@fig:029])

![Проверка](image/29.png){#fig:029 width=70%}

Проверяем устраивают ли нас изменения, дальше принимаем их. (рис. [-@fig:030])

![Принятие изменений](image/30.png){#fig:030 width=70%}

Применяем изменения. (рис. [-@fig:031])

![Принятие изменений](image/31.png){#fig:031 width=70%}

Устанавливаем свои dotfiles на новую виртуальную машину одной командной. (рис. [-@fig:032])

![Установка](image/32.png){#fig:032 width=70%}

Можно извлечь изменения из репозитория и применить их одной командой. (рис. [-@fig:033])

![Извлечение и применение](image/33.png){#fig:033 width=70%}

Извлечем последние изменения из нашего репозитория и посмотрим, что изменится, фактически не применяя изменения. (рис. [-@fig:034])

![Просмотр изменений](image/34.png){#fig:034 width=70%}

Если мы довольны изменениями, применим их. (рис. [-@fig:035])

![Применение изменений](image/35.png){#fig:035 width=70%}

Включаем автоматическое фиксирование и отправление изменений в исходный каталог в репозиторий. (рис. [-@fig:036])

![Включение автоматического фиксирования и отправления](image/36.png){#fig:036 width=70%}

# Выводы

C помощью данной лабораторной работы я создала удобное рабочее пространство для дальнейшего использования.
