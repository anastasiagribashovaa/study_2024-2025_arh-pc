---
## Front matter
title: "Отчет по лабораторной работе №2"
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

Изучение идеологии, применение средств контроля версий и обретение практических
навыков по работе с системой git.

# Задание

Используя методические материалы, провести работу, состоящую из настройки git и
создания репозитория.


# Теоретическое введение

Системы контроля версий (Version Control System, VCS) применяются при работе нескольких человек над одним проектом. Обычно основное дерево проекта хранится в локальном или удалённом репозитории, к которому настроен доступ для участников проекта. При внесении изменений в содержание проекта система контроля версий позволяет их фиксировать, совмещать изменения, произведённые разными участниками проекта, производить откат к любой более ранней версии проекта, если это требуется.
В классических системах контроля версий используется централизованная модель, предполагающая наличие единого репозитория для хранения файлов. Выполнение большинства функций по управлению версиями осуществляется специальным сервером. Участник проекта (пользователь) перед началом работы посредством определённых команд получает нужную ему версию файлов. После внесения изменений, пользователь размещает новую версию в хранилище. При этом предыдущие версии не удаляются из центрального хранилища и к ним можно вернуться в любой момент. Сервер может сохранять не полную версию изменённых файлов, а производить так называемую дельта-компрессию — сохранять только изменения между последовательными версиями, что позволяет уменьшить объём хранимых данных.

# Выполнение лабораторной работы

Открываю терминал и делаю предварительную конфигурацию git; затем настраиваю utf-8 в выводе сообщений git (рис. 4.3.2); далее задаю имя начальной ветки, после чего ввожу параметры autocrlf и safecrlf (рис. [-@fig:001]).

(image/photo_5212962752920939089_Y-jpg){#fig:001 width=70%}

Генерирую пару ключей(приватный и открытый) для последующей идентификации пользователя на сервере репозиториев и копирую из локальной консоли в буфер обмена; затем захожу на GitHub и вставляю SSH ключ в нужное поле на сайте (рис. [-@fig:002]).

(image/photo_52129627 52920939090_y.jpg){#fig:002 width=70%}

Открываю терминал и создаю каталог для предмета «Архитектура компьютера» (рис. [-@fig:003]).

(image/photo_5212962752920939091_y-jpg){#fig:003 width=70%}

Перехожу на страницу репозитория с шаблоном курса по ссылке, указанном в инструкции к лабораторной работе, нажимаю кнопку «use this temple», задаю имя репозитория и создаю его; далее открываю терминал, перехожу в каталог курса и копирую созданный репозиторий с помощью команды git clone (рис. [-@fig:004]).

(image/photo_52129627 52920939092_y.jpg){#fig:004 width=70%}

Перехожу в каталог курса; удаляю лишние файлы с помощью команды rm; создаю необходимые каталоги (рис. 4.7.3); отправляю файлы на сервер (рис. 4.7.4); в конце проверяю правильность на странице github (рис. [-@fig:005]).

(image/photo_5212962752920939093_Yjpg){#fig:005 width=70%}


# Задания для самостоятельной работы
Задание 1
Создаю каталоги ~/work/study/2024-2025/«Архитектура компьютера»/arch-pc/labs/lab01/report и ~/work/study/2024-2025/«Архитектура компьютера»/arch-pc/labs/lab02/report с помощью команды mkdir, после чего создаю отчет по выполнению лабораторной работы в каталоге labs/lab02/report (рис. [-@fig:006]).

(image/photo_5212962752920939094_y-jpg){#fig:006 width=70%}

Задание 2
Копирую отчеты по выполнению предыдущей лабораторной работы в каталог labs/lab01/report (рис. [-@fig:007]).

image/photo_5212962752920939095_y.jpg){#fig:007 width=70%}

Задание 3
Загружаю файлы на github, используя команды git add, git commit -m и git push -f origin master (рис. 5.3.1) и проверяю правильность выполнения задания (рис. [-@fig:008]).

image/photo_5212962752920939097_y.jpg){#fig:008 width=70%}


# Выводы

При выполнении данной лабораторной работы я приобрела навыки по работы с
системой git, а также изучила идеологию и применение средств контроля версий.


# Список литературы{.unnumbered}

1. https://esystem.rudn.ru/mod/resource/view.php?id=1030550
2. https://esystem.rudn.ru/mod/page/view.php?id=1030492
3. https://esystem.rudn.ru/mod/resource/view.php?id=1030496
