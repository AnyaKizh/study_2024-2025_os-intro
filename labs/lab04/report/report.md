---
## Front matter
title: "Oтчёт по лабораторной работе 4"
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

Получение практических навыков правильной работы с репозиторием git.

# Выполнение лабораторной работы

Описываются проведённые действия, в качестве иллюстрации даётся ссылка на иллюстрацию (рис. [-@fig:001]).


Заходим в виртуальную машину и открываем консоль с помощью комбинации Win+Enter. (рис. [-@fig:001])

![Консоль](image/1.png){#fig:001 width=70%}

Устанавливаем git-flow. (рис. [-@fig:002])

![Установка git-flow](image/2.png){#fig:002 width=70%}

Устанавливаем Node.js. (рис. [-@fig:003] рис. [-@fig:004])

![Установка Node.js](image/3.png){#fig:003 width=70%}

![Установка Node.js](image/4.png){#fig:004 width=70%}

Для работы с Node.js добавим каталог с исполняемыми файлами, устанавливаем yarn, в переменную path. (рис. [-@fig:005] рис. [-@fig:006])

![Настройка Node.js](image/5.png){#fig:005 width=70%}

![Настройка Node.js](image/6.png){#fig:006 width=70%}

Устанавливаем программу для помощи в форматировании коммитов. (рис. [-@fig:007])

![Установка программы](image/7.png){#fig:007 width=70%}

Устанавливаем Standard-changelog для помощи в создании логов. (рис. [-@fig:008])

![Установка программы](image/8.png){#fig:008 width=70%}

Создаем репозиторий на GitHub. Называем его git-extended. (рис. [-@fig:009])

![Создание репозитория](image/9.png){#fig:009 width=70%}

Делаем первый коммит и выкладываем на github. (рис. [-@fig:010])

![Первый коммит](image/10.png){#fig:010 width=70%}

Делаем конфигурацию для пакетов Node.js. Необходимо заполнить несколько параметров пакета. (рис. [-@fig:011])

![Конфигурация Node.js](image/11.png){#fig:011 width=70%}

Сконфигурируем формат коммитов. Для этого добавим в файл package.json команду для формирования 
коммитов. (рис. [-@fig:012])

![Добавление команды для формирования коммитов](image/12.png){#fig:012 width=70%}

Добавим новые файлы. (рис. [-@fig:013])

![Добавление новых файлов](image/13.png){#fig:013 width=70%}

Выполняем коммит. (рис. [-@fig:014])

![Выполнение коммита](image/14.png){#fig:014 width=70%}

Отправляем на github. (рис. [-@fig:015])

![Отправка на github](image/15.png){#fig:015 width=70%}

Переходим к конфигурации git-flow. Инициализируем git-flow. (рис. [-@fig:016])

![Инициализация git-flow](image/16.png){#fig:016 width=70%}

Префикс для ярлыков установим в v.

Проверяем, что мы на ветке develop. (рис. [-@fig:017])

![Проверка ветки](image/17.png){#fig:017 width=70%}

Загружаем весь репозиторий в хранилище. (рис. [-@fig:018])

![Загрузка репозитория в хранилище](image/18.png){#fig:018 width=70%}

Устанавливаем внешнюю ветку как вышестоящую для этой ветки. (рис. [-@fig:019])

![Установка внешней ветки](image/19.png){#fig:019 width=70%}

Создадим релиз с версией 1.0.0. (рис. [-@fig:020])

![Создание релиза](image/20.png){#fig:020 width=70%}

Создадим журнал изменений. (рис. [-@fig:021])

![Создание журнала изменений](image/21.png){#fig:021 width=70%}

Добавим журнал изменений в индекс. (рис. [-@fig:022])

![Добавление журнала изменений](image/22.png){#fig:022 width=70%}

Зальём релизную ветку в основную ветку. (рис. [-@fig:023])

![Добавление релизной ветки](image/23.png){#fig:023 width=70%}

Отправим данные на GitHub. (рис. [-@fig:024])

![Отправка данных](image/24.png){#fig:024 width=70%}

Создадим релиз на GitHub. Для этого используем утилиты работы с Github. (рис. [-@fig:025])

![Создание релиза](image/25.png){#fig:025 width=70%}

Создадим ветку для новой функциональности. Объединим созданную ветку с develop. (рис. [-@fig:026])

![Создание новой ветки и объединение со старой](image/26.png){#fig:026 width=70%}

Перейдем к созданию релиза git-flow. Создадим релиз с версией 1.2.3. (рис. [-@fig:027])

![Создание релиза](image/27.png){#fig:027 width=70%}

Обновим номер версии в файле package.json. Установим её в 1.2.3. (рис. [-@fig:028])

![Обновление номера версии](image/28.png){#fig:028 width=70%}

Создадим журнал изменений. (рис. [-@fig:029])

![Создание журнала изменений](image/29.png){#fig:029 width=70%}

Добавим журнал изменений в индекс. (рис. [-@fig:030])

![Добавление журнала изменений](image/30.png){#fig:030 width=70%}

Зальём релизную ветку в основную ветку. (рис. [-@fig:031])

![Добавление релизной ветки в основную](image/31.png){#fig:031 width=70%}

Отправляем данные на GitHub. (рис. [-@fig:032])

![Отправка данных на GitHub](image/32.png){#fig:032 width=70%}

Создадим релиз на GitHub с комментарием из журнала изменений. (рис. [-@fig:033])

![Создание релиза](image/33.png){#fig:033 width=70%}

# Выводы

В ходе лабораторной работы я получила навыки правильной работы с репозиторием git.
