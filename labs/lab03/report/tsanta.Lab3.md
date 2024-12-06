---
## Front matter
title: "Oтчёт по лабораторной работе 03"
subtitle: "НММбд-04-24"
author: "Ракутуманандзара Цантамписедрана Сарубиди"

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

Целью данной лабораторной работы является освоение процедуры оформления отчетов с помощью легковесного языка разметки Markdown.

# Задание

   1. Установка необходимого ПО

   2. Заполнение отчета по выполнению лабораторной работы No4 с помощью языка разметки Markdown

   3. Задание для самостоятельной работы


# Теоретическое введение

При выполнении лабораторной работы на своей технике необходимо установить следующее ПО:
• TeX Live (https://www.tug.org/texlive/) последней версии.
• Pandoc (https://pandoc.org/).
На компьютерах в дисплейных классах факультета физико-математических и естествен-
ных наук РУДН все необходимое ПО установлено.

# Выполнение лабораторной работы

Заполнение отчета по выполнению лабораторной работы No.3 с помощью языка разметки Markdown. I open the terminal. I go to the course catalog created during the previous laboratory work(рис 1) (рис. [-@fig:001]).

![ previous laboratory work]( image/001.png){#fig:001 width=70%}



Я обновляю локальный репозиторий, скачав изменения из удаленного репозитория с помощью команды git pull(рис 2).

![ git pull ]( image/002.png){#fig:002 width=70%}



Я перейду в каталог с отчётом No.3 с помощью команду cd(рис 3).

![ каталог с отчётом No.3 ]( image/003.png){#fig:003 width=70%}



Я компилирую шаблон с использованием Makefile, вводя команду make(рис 4).

![ Makefile ]( image/004.png){#fig:004 width=70%}



Я открываю сгенерированные файлы report.docx LibreOffice и report pdf(рис 5)

![ report.pdf ]( image/005.png){#fig:005 width=70%}


Полученные файлы я удалю с помощью Makefile, введя команду make clean. Командой ls проверяю, удалены ли созданные файлы(рис 6).


![ make clean ]( image/006.png){#fig:006 width=70%}


Я открываю файл report.md с помощью любого текстового редактор(рис 16)


![report.md ]( image/007.png){#fig:007 width=70%}



Я хочу, чтобы у меня на всякий случай сохранился шаблон отчета, поэтому копирую файл с новым названием с помощью команду cp(рис 8)


![шаблон отчета ]( image/008.png){#fig:008 width=70%}



Я начинаю заполнять отчет с помощью языка разметки Markdown в скопированном файле(рис 9).


![заполнять отчет ]( image/009.png){#fig:009 width=70%}


Задание для самостоятельной работы Я перейду в каталог lab02/report с помощью команды cd(рис 10).

![каталог lab02 ]( image/0010.png){#fig:0010 width=70%}


Я изменю имя с report.md на tsanta.lab2.md с помощью команды cp и запущу команду make(рис 11).


![make ]( image/0011.png){#fig:0011 width=70%}



Я открываю файл с помощью текстового редактора и начинаю заполнять отчет(рис 12).


![ заполнять отчет ]( image/0012.png){#fig:0012 width=70%}



Я компилирую файл с отчетом по лабораторной работе(рис 13)

![ компия файла ]( image/0013.png){#fig:0013 width=70%}


Я удаляю сгенерированные фаилы report.docx и report.pdf(рис 14)

![ yдалить сгенерированные фаилы ]( image/0014.png){#fig:0014 width=70%}


Я добавляю изменения на GitHub с помощью комнадой git add и сохраняю изменения с помощью commit(рис 15)


![ git add ]( image/0015.png){#fig:0015 width=70%}



Я отправлялю файлы на сервер с помощью команды git pull(рис 16)


![ git pull ]( image/0016.png){#fig:0016 width=70%}




# Выводы
В результате выполнения данной лабораторной работы я освоила процедуры оформления отчетов с помощью легковесного языка разметки Markdown.

# Список литературы{.unnumbered}

1. Архитектура ЭВМ

