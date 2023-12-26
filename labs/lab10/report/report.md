---
## Front matter
title: "Лабораторная работа №10"
subtitle: "Работа с файлами средствами Nasm"
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

Целью работы является приобретение навыков написания программ для работы с файлами.

# Выполнение лабораторной работы

Я создал директорию для выполнения лабораторной работы номер 10 и перешел в нее. В этой директории были созданы три файла: lab10-1.asm, readme-1.txt и readme-2.txt.

В файле lab10-1.asm я разработал программу согласно примеру 10.1, которая осуществляет запись текстового сообщения в файл. Затем скомпилировал этот исходный код в исполняемый файл и осуществил проверку его функционирования (см. рисунок [-@fig:001]).

![Программа в файле lab10-1.asm](image/01.png){ #fig:001 width=70%, height=70% }

Эта программа запрашивает ввод текстовой строки и записывает ее в файл readme.txt. В случае отсутствия данного файла, вводимая строка не будет сохранена (см. рисунок [-@fig:002]).

![Запуск программы lab10-1.asm](image/02.png){ #fig:002 width=70%, height=70% }

Тем не менее, запустить файл не удалось, поскольку из-за отсутствия атрибута "x" запрещено его выполнение (см. рисунок [-@fig:003]).

![Запуск запрещен](image/03.png){ #fig:003 width=70%, height=70% }

Я изменил разрешения файла lab10-1.asm, вновь добавив права на выполнение с помощью команды chmod. После этой операции я снова попытался запустить файл (см. рисунок [-@fig:004]).

В итоге файл был запущен, и система попыталась интерпретировать его содержимое как набор команд командной строки. Однако, поскольку файл содержит код на языке ассемблера, а не команды оболочки, возникли ошибки. Но если бы в файле были команды оболочки, их можно было бы выполнить, запустив файл.

![Файл с кодом с разрешением запуска](image/04.png){ #fig:004 width=70%, height=70% }

Затем я установил права доступа к файлам readme в соответствии с вариантом, представленным в таблице 10.4. Для проверки корректности настройки прав я использовал команду ls -l (см. рисунок [-@fig:005]).
для варианта 14: ```r-x rwx rwx``` ```110 111 110```

![Установка прав](image/05.png){ #fig:005 width=70%, height=70% }

## Задание для самостоятельной работы

Написал программу работающую по следующему алгоритму (рис. [-@fig:006]) (рис. [-@fig:007]):

* Вывод приглашения “Как Вас зовут?”

* ввести с клавиатуры свои фамилию и имя

* создать файл с именем name.txt

* записать в файл сообщение “Меня зовут”

* дописать в файл строку введенную с клавиатуры

* закрыть файл

![Программа в файле lab10-2.asm](image/06.png){ #fig:006 width=70%, height=70% }

![Запуск программы lab10-2.asm](image/07.png){ #fig:007 width=70%, height=70% }

# Выводы

Освоили работy с файлами и правами доступа.

# Список литературы{.unnumbered}

1. GDB: The GNU Project Debugger. — URL: https://www.gnu.org/software/gdb/.

2. GNU Bash Manual. — 2016. — URL: https://www.gnu.org/software/bash/manual/.

3. Midnight Commander Development Center. — 2021. — URL: https://midnight-commander.org/.

4. NASM Assembly Language Tutorials. — 2021. — URL: https://asmtutor.com/.

5. Newham C. Learning the bash Shell: Unix Shell Programming. — O’Reilly Media, 2005. — 354 с. — (In a Nutshell). — ISBN 0596009658. — URL: http://www.amazon.com/Learning-bash-Shell-Programming-Nutshell/dp/0596009658.

6. Robbins A. Bash Pocket Reference. — O’Reilly Media, 2016. — 156 с. — ISBN 978-1491941591.

7. The NASM documentation. — 2021. — URL: https://www.nasm.us/docs.php.

8. Zarrelli G. Mastering Bash. — Packt Publishing, 2017. — 502 с. — ISBN 9781784396879.

9. Колдаев В. Д., Лупин С. А. Архитектура ЭВМ. — М. : Форум, 2018.

10. Куляс О. Л., Никитин К. А. Курс программирования на ASSEMBLER. — М. : Солон-Пресс, 2017.

11. Новожилов О. П. Архитектура ЭВМ и систем. — М. : Юрайт, 2016.

12. Расширенный ассемблер: NASM. — 2021. — URL: https://www.opennet.ru/docs/RUS/nasm/.

13. Робачевский А., Немнюгин С., Стесик О. Операционная система UNIX. — 2-е изд. — БХВ Петербург, 2010. — 656 с. — ISBN 978-5-94157-538-1.

14. Столяров А. Программирование на языке ассемблера NASM для ОС Unix. — 2-е изд. — М. : МАКС Пресс, 2011. — URL: http://www.stolyarov.info/books/asm_unix.

15. Таненбаум Э. Архитектура компьютера. — 6-е изд. — СПб. : Питер, 2013. — 874 с. — (Классика Computer Science).

16. Таненбаум Э., Бос Х. Современные операционные системы. — 4-е изд. — СПб. : Питер, 2015. — 1120 с. — (Классика Computer Science).