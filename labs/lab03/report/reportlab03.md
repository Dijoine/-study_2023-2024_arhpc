---
## Front matter
title: "Шаблон отчёта по лабораторной работе"
subtitle: "Простейший вариант"
author: "Дмитрий Сергеевич Холхов"

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
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
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

Целью работы является освоение процедуры оформления отчетов с помощью легковесного языка разметки Markdown.

# Выполнение лабораторной работы

Я открыл терминал, перешёл в каталог arch-pc, обновил локальный репозиторий, введя git pull, перешёл в каталог с шаблоном отчета по лабораторной работе №3 (рис. [-@fig:001]).

![Обновление терминала и перемещение между директориями](/afs/.dk.sci.pfu.edu.ru/home/d/s/dskhokhlov/work/study/2023-2024/Архитектура компьютера/-study_2023-2024_arhpc/labs/lab03/report/image/Снимок экрана от 2023-10-13 18-05-51.png){ #fig:001 width=70% }

Провожу компиляцию шаблона и проверяю корректность выполнения команды (рис. [-@fig:002]).

![Компиляция шаблона](/afs/.dk.sci.pfu.edu.ru/home/d/s/dskhokhlov/work/study/2023-2024/Архитектура компьютера/-study_2023-2024_arhpc/labs/lab03/report/image/Снимок экрана от 2023-10-13 18-07-22.png){ #fig:002 width=70% }

Удаляю полученные файлы и проверяю, что файлы были удалены (рис. [-@fig:003]).

![Удаление файлов](/afs/.dk.sci.pfu.edu.ru/home/d/s/dskhokhlov/work/study/2023-2024/Архитектура компьютера/-study_2023-2024_arhpc/labs/lab03/report/image/Снимок экрана от 2023-10-13 18-08-35.png){ #fig:003 width=70% }

Открываю файл report.md с помощью текстового редактора (рис. [-@fig:004]).

![Открытие файла с шаблоном отчета](/afs/.dk.sci.pfu.edu.ru/home/d/s/dskhokhlov/work/study/2023-2024/Архитектура компьютера/-study_2023-2024_arhpc/labs/lab03/report/image/Снимок экрана от 2023-10-13 18-08-47.png){ #fig:004 width=70% }

# Выполнение заданий для самостоятельной работы

Перехожу в каталог с отчетом по третьей лабораторной работе (рис. [-@fig:005]).

![Перемещение между директориями](/afs/.dk.sci.pfu.edu.ru/home/d/s/dskhokhlov/work/study/2023-2024/Архитектура компьютера/-study_2023-2024_arhpc/labs/lab03/report/image/Снимок экрана от 2023-10-13 20-05-47.png){ #fig:005 width=70% }

Открыл файл с шаблоном отчета и заполнила его (рис. [-@fig:006]).

![Открытие файла с шаблоном отчета](/afs/.dk.sci.pfu.edu.ru/home/d/s/dskhokhlov/work/study/2023-2024/Архитектура компьютера/-study_2023-2024_arhpc/labs/lab03/report/image/Снимок экрана от 2023-10-13 20-12-15.png){ #fig:006 width=70% }

Переименовал файл, в котором заполнил отчет (рис. [-@fig:007]).

![Переименование файла](/afs/.dk.sci.pfu.edu.ru/home/d/s/dskhokhlov/work/study/2023-2024/Архитектура компьютера/-study_2023-2024_arhpc/labs/lab03/report/image/Снимок экрана от 2023-10-13 20-16-05.png){ #fig:007 width=70% }

Загружаю файлы на GitHub (рис. [-@fig:008]).

![Добавление файлов на GitHub](/afs/.dk.sci.pfu.edu.ru/home/d/s/dskhokhlov/work/study/2023-2024/Архитектура компьютера/-study_2023-2024_arhpc/labs/lab03/report/image/Снимок экрана от 2023-10-13 20-41-15.png){ #fig:008 width=70% }

# Выводы

Я освоил процедуры оформления отчетов с помощью легковесного языка разметки Markdown.

