---
## Front matter
title: "Oтчёта по лабораторной работе 4"
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
    2. Заполнение отчета по выполнению лабораторной работы №4 с помощью языка разметки Markdown
    3. Задание для самостоятельной работы


# Теоретическое введение

Markdown - легковесный язык разметки, созданный с целью обозначения форматирования в простом тексте, с максимальным сохранением его читаемости человеком, и пригодный для машинного преобразования в языки для продвинутых публикаций. Внутритекстовые формулы делаются аналогично формулам LaTeX. В Markdown вставить изображение в документ можно с помощью непосредственного указания адреса изображения. Синтаксис Markdown для встроенной ссылки состоит из части [link text], представляющей текст гиперссылки, и части (file-name.md) – URL-адреса или имени файла, на который дается ссылка. Markdown поддерживает как встраивание фрагментов кода в предложение, так и их размещение между предложениями в виде отдельных огражденных блоков. Огражденные блоки кода — это простой способ выделить синтаксис для фрагментов кода.

# Выполнение лабораторной работы

##1 Создание программы Hello world!

я буду использовать mkdir для создания указанного каталога, а затем с помощью команды cd войду в каталог, в котором буду работать, там я создам пустой текстовый файл «hello.asm» с помощью команды touch (рис 1).

![ рис 1 ](image/001.png){#fig:001 width=70%}


Я открываю созданный файл в текстовом редакторе и заполню файл, вставив в него программу вывода «Hello word!» (рис 2).

![ рис 2 ](image/002.png){#fig:002 width=70%}

##2 Транслятором NASM

Я преобразую текст программы в вывод «Hello world!» в объектный код с помощью транслятора NASM с помощью команды nasm -f elf hello.asm. Далее проверяю правильность выполнения команды с помощью команды ls и, как показано, файл hello.o создан (рис3).

![ рис3 ](image/003.png){#fig:003 width=70%}

##3 Расширенным синтаксисом командной строки NASM

Я введу команду, которая скомпилирует файл hello.asm в файл obj.o, и файл будет содержать символы отладки (переключатель -g), также используя переключатель -l будет создан файл листинга list.lst. Далее проверяю с помощью команды ls правильность выполнения команды(рис 4)

![ рис4 ](image/004.png){#fig:004 width=70%}

##4 Компоновщиком LD

Я передам объектный файл hello.o для обработки компоновщиком LD для создания исполняемого файла hello. Далее я использую команду ls, чтобы проверить правильность выполнения команды(рис 5).

![ рис 5 ](image/005.png){#fig:005 width=70%}

Теперь я создам файл с именем «main» с помощью данной команды.Объектный файл, из которого собран этот исполняемый файл, имеет имя obj.o(рис 6)

![ рис 6 ](image/006.png){#fig:006 width=70%}

##5 Запуск исполняемого файла

Я запущу созданный исполняемый файл hello(рис 7)

![ рис 7 ](image/007.png){#fig:007 width=70%}

##6 Выполнение заданий для самостоятельной работы.

С помощью команды cp я создам копию файла hello.asm в текущем каталоге с именем lab4.asm(рис 8).

![ рис 8 ](image/008.png){#fig:008 width=70%}

C помощью текстового редактора я открою файл lab4.asm и внесу изменения в программу, чтобы она отображала мое имя и фамилию(рис 9)

![ рис 9 ](image/009.png){#fig:009 width=70%}


Текст программы я скомпилирую в объектный файл. С помощью команды ls я проверяю, что файл lab5.o создан(рис 10)

![ рис 10 ](image/0010.png){#fig:0010 width=70%}


Я передам объектный файл lab5.o компоновщику LD для обработки для создания исполняемого файла lab5(рис 11).

![ рис 11 ](image/0011.png){#fig:0011 width=70%}


Когда я запускаю исполняемый файл lab4, мое имя и фамилия фактически отображаются на экране(рис 13)

![ рис 12 ](image/0012.png){#fig:0012 width=70%}


Я скопирую файлы hello.asm и lab4.asm в свой локальный репозиторий в каталоге ~/work/study/2023-2024/"Архитектура компьютера"/arch-pc/labs/lab04/report. Я сделаю это с помощью команды cd(рис 13)

![ рис 13 ](image/0013.png){#fig:0013 width=70%}

Используя команду git add и git commit, я добавлю файлы в github(рис 14)

![ рис 14 ](image/0014.png){#fig:0014 width=70%}


Я отправляю файлы на сервер с помощью команды git push(рис 15)

![ рис 15 ](image/0015.png){#fig:0015 width=70%}




# Выводы

При выполнении данной лабораторной работы я освоила процедуры компиляции и сборки программ, написанных на ассемблере NASM.

# Список литературы{.unnumbered}

Архитектура ЭВМ
