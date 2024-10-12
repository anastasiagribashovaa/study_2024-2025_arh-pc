---
## Front matter
title: "Отчёт по лабораторной работе №3"
subtitle: "Дисциплина: Архитектура компьютера"
author: "Грибашова Анастасия Александровна"

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
fontsize: 13pt
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

Освоение процедуры оформления отчетов с помощью легкословесного языка Markdown.

# Задание

1. Установление неоюходимого ПО.
2. Зполнение отчета по лабораторной работе с помощью языка Markdown.
3. Задания для самостоятельной работы.

# Теоретическое введение
Markdown - легковесный язык разметки, созданный с целью обозначения форматирования в простом тексте, с максимальным сохранением его читаемости человеком, и пригодный для машинного преобразования в языки для продвинутых публикаций. Внутритекстовые формулы делаются аналогично формулам LaTeX. В Markdown вставить изображение в документ можно с помощью непосредственного указания адреса изображения. Синтаксис Markdown для встроенной ссылки состоит из части [link text], представляющей текст гиперссылки, и части (file-name.md) – URL-адреса или имени файла, на который дается ссылка. Markdown поддерживает как встраивание фрагментов кода в предложение, так и их размещение между предложениями в виде отдельных огражденных блоков. Огражденные блоки кода — это простой способ выделить синтаксис для фрагментов кода.

# Выполнение лабораторной работы

Открываю терминал и перехожу в каталог arch-pc (рис. [-@fig:001]).

(image/photo_5212962752920938805_y-jpg){#fig:001 width=70%}

Обновляю локальный репозиторий, скачав изменения из удаленного репозитория с помощью команды git pull (рис. [-@fig:002]).

(image/photo_5212962752920938806_y-jpg){#fig:002 width=70%}

Перехожу в каталог с шаблоном отчета по лабораторной работе № 3 (рис. [-@fig:003]).

(image/photo_5212962752920938807 _y-jpg){#fig:003 width=70%}

Провожу компиляцию шаблона с использованием Makefile с помощью команды make и проверяю правильность выполнения команды (рис. [-@fig:004]).

(image/photo_5212962752920938808_y-jpg){#fig:004 width=70%}

Удаляю полученные файлы с помощью команды make clean и проверяю правильность выполенения (рис. [-@fig:005]).

(image/photo_5212962752920938809_y-jpg){#fig:005 width=70%}

Откпрываю файл report.mdc с помощью gedit и затемп заполняю его (рис. [-@fig:006]).

(image/photo_5212962752920938810_y-jpg){#fig:006 width=70%}



# Выводы

Благодаря данной лабораторной работе я освоила процедуры оформления отчетов с помощью языка разметки Markdown.

# Список литературы{.unnumbered}

Курс по архитектуре компьютера.
