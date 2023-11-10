---
## Front matter
title: "Отчёта по лабораторной работе №5"
subtitle: "Основы работы с Midnight Commander"
author: "Семенов Сергей Алексеевич"

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
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Освоить инструкции языка ассемблера mov.Приобрести знания использования Midnight Commander.

# Задание
Написать 2 программы по примеру и впоследствии изменить их по условию.
# Выполнение лабораторной работы
![Окно midnight commander](image/1.png)

Открываем midnight commander

![Создание каталога в midnight commander](image/2.png)

Создаем каталог

![редактор nano](image/3.png)

Создание редактора nano

![Листинг 5.1](image/4.png)

Листинг 5.1

![Создание копии файла](image/5.png)

Создали копию файла

![Листинг 5.2](image/6.png)

Листинг 5.2

![sprintLF](image/7.png)

sprintLF

Написать 2 программы по примеру и впоследствии изменить их по условию.
## Порядок выполнения лабораторной работы

Таким образом можем понять, что команда sprint выводит текст в той же строке, а sprintLF переносит на новую строку.

## Задание для самостоятельной работы
![Изменённая программа для вывода текста на экран](image/8.png)

![Изменённая программа №1](image/9.png)

![Измененная программа №2](image/10.png)

![Рабочая программа](image/11.png)

# Выводы

Мы приобрели навыки работы с Midnight Commander и осоили инструкции mov.

