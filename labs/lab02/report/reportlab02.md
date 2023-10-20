---
## Front matter
title: "Шаблон отчёта по лабораторной работе 2"
subtitle: "Простейший вариант"
author: "Дмитрий Сергеевич Хохлов"

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

Изучить идеологию и применение средств контроля версий.
Приобрести практические навыки по работе с системой git. 

# Выполнение лабораторной работы

Захожу на GitHub (рис. [-@fig:001]).

![Зашёл на гитхаб](/afs/.dk.sci.pfu.edu.ru/home/d/s/dskhokhlov/work/study/2023-2024/Архитектура компьютера/-study_2023-2024_arhpc/labs/lab02/report/image/Снимок экрана от 2023-09-27 12-41-44.png){ #fig:001 width=70% }

Открываю консоль и начинаю базовую настройку Git (рис. [-@fig:002]).

![Базовая настройка гитхаба](/afs/.dk.sci.pfu.edu.ru/home/d/s/dskhokhlov/work/study/2023-2024/Архитектура компьютера/-study_2023-2024_arhpc/labs/lab02/report/image/Снимок экрана от 2023-09-27 13-01-33.png){ #fig:002 width=70% }

Генерирую ssh-ключ (рис. [-@fig:003]).

![Генерация SSH-ключа](/afs/.dk.sci.pfu.edu.ru/home/d/s/dskhokhlov/work/study/2023-2024/Архитектура компьютера/-study_2023-2024_arhpc/labs/lab02/report/image/Снимок экрана от 2023-09-27 13-18-04.png){ #fig:003 width=70% }

Добавляю этот ключ в GitHub (рис. [-@fig:004]).

![Добавление SSH-ключа в Гит](/afs/.dk.sci.pfu.edu.ru/home/d/s/dskhokhlov/work/study/2023-2024/Архитектура компьютера/-study_2023-2024_arhpc/labs/lab02/report/image/Снимок экрана от 2023-10-13 18-55-14.png){ #fig:004 width=70% }

Создаю каталог для предмета «Архитектура компьютера»  (рис. [-@fig:005]).

![Создание кактлога](/afs/.dk.sci.pfu.edu.ru/home/d/s/dskhokhlov/work/study/2023-2024/Архитектура компьютера/-study_2023-2024_arhpc/labs/lab02/report/image/Снимок экрана от 2023-10-13 18-56-44.png){ #fig:005 width=70% }

Клонирую созданный репозиторий (рис. [-@fig:006]).
 
![Клонирование созданного репозитория](/afs/.dk.sci.pfu.edu.ru/home/d/s/dskhokhlov/work/study/2023-2024/Архитектура компьютера/-study_2023-2024_arhpc/labs/lab02/report/image/Снимок экрана от 2023-10-13 18-58-45.png){ #fig:006 width=70% }

Проверяю, что всё хорошо (рис. [-@fig:007]).

![Проверка](/afs/.dk.sci.pfu.edu.ru/home/d/s/dskhokhlov/work/study/2023-2024/Архитектура компьютера/-study_2023-2024_arhpc/labs/lab02/report/image/Снимок экрана от 2023-10-13 18-59-06.png){ #fig:007 width=70% }

Удаляю лишние файлы (рис. [-@fig:008]).

![Удаление лишних файлов](/afs/.dk.sci.pfu.edu.ru/home/d/s/dskhokhlov/work/study/2023-2024/Архитектура компьютера/-study_2023-2024_arhpc/labs/lab02/report/image/Снимок экрана от 2023-10-13 18-59-36.png){ #fig:008 width=70% }

Создаю необходимые каталоги и отправляю их на сервер (рис. [-@fig:009]).

![Создание каталогов](/afs/.dk.sci.pfu.edu.ru/home/d/s/dskhokhlov/work/study/2023-2024/Архитектура компьютера/-study_2023-2024_arhpc/labs/lab02/report/image/Снимок экрана от 2023-10-13 19-01-06.png){ #fig:009 width=70% }

#Самостоятельная работа

1. Создаю отчет по выполнению лабораторной работы
в соответствующем каталоге рабочего пространства
(labs>lab02>report).
2. Копирую отчеты по выполнению предыдущих
лабораторных работ в соответствующие каталоги созданного
рабочего пространства.
3. Загружаю файлы на github (рис. [-@fig:010]).
image/Сним
![Выполнение самостоятельной работы](/afs/.dk.sci.pfu.edu.ru/home/d/s/dskhokhlov/work/study/2023-2024/Архитектура компьютера/-study_2023-2024_arhpc/labs/lab02/report/image/Снимок экрана от 2023-10-13 19-01-33.png){ #fig:010 width=70% }

#Вывод 

По итогам данной лабораторной работы я изучил идеологию
CVS (Git). И приобрёл навык работы с ним.

