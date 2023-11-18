---
## Front matter
title: "Отчёта по лабораторной работе №6"
subtitle: "Арифметические операции в NASM."
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

Освоить арифметических инструкций языка ассемблера NASM и написать программы для вычисления арифметических выражений с неизвестной.

# Задание

Написать программы для решения выражений.

# Выполнение лабораторной работы

## Cимвольные и численные данные в NASM

Создаем каталог для программ ЛБ6, и в нем создаем файл

![Создаем каталог с помощью команды mkdir и файл с помощью команды touch](image/1.jpg)

Открываем файл в Midnight Commander и заполняем его в соответствии с листингом 6.1

![Заполняем файл](image/2.jpg)

Создаем исполняемый файл и запускаем его.

![Запускаем файл и смотрим на его работу](image/3.jpg)

Снова открываем файл для редактирования и убиравем кавычки с числовых значений

![Изменяем файл](image/4.jpg)

Создаем исполняемый файл и запускаем его

![Запускаем файл и смотрим на его работу](image/5.jpg)

Создаем новый файл в каталоге

![Создаем файл](image/6.jpg)

Заполняем файл в соответствии с листингом 6.2

![Заполняем файл](image/7.jpg)

Создаем исполняемый файл и запускаем его

![Смотрим на работу программы](image/8.jpg)

Снова открываем файл для редактирования и убиравем кавычки с числовых значений

![Изменяем файл](image/9.jpg)

Создаем исполняемый файл и запускаем его

![Смотрим на работу программы](image/10.jpg)

Вывод функций iprintLF и iprint отличаются только тем, что LF переносит на новую строку.

## Выполнение арифметических операций в NASM

Открываем файл и редактируем в соответствии с листингом 6.3

![Заполняем файл](image/11.jpg)

Создаем исполняемый файл и запускаем

![Смотрим на результат работы программы](image/12.jpg)

Компилируем файл и запускаем программу

![Смотрим на результат работы программы](image/13.jpg)

Компилируем файл и запускаем его

![Проверяемс результат работы программы](image/14.jpg)

## Ответы на вопросы по программе

1. Строка "mov eax,rem" и строка "call sprint" отвечают за вывод на экран сообщения ‘Ваш вариант:'.

2. Эти инструкции используются для чтения строки с вводом данных от пользователя. Начальный адрес строки сохраняется в регистре ecx, а количество символов в строке (максимальное количество символов, которое может быть считано) сохраняется в регистре edx. Затем вызывается процедура sread, которая выполняет чтение строки.

3. Инструкция "call atoi" используется для преобразования строки в целое число. Она принимает адрес строки в регистре eax и возвращает полученное число в регистре eax.

4. Строка "xor edx,edx" обнуляет регистр edx перед выполнением деления. Строка "mov ebx,20" загружает значение 20 в регистр ebx. Строка "div ebx" выполняет деление регистра eax на значение регистра ebx с сохранением частного в регистре eax и остатка в регистре edx.

5. Остаток от деления записывается в регистр edx.

6. Инструкция "inc edx" используется для увеличения значения в регистре edx на 1. В данном случае, она увеличивает остаток от деления на 1.

7. Строка "mov eax,edx" передает значение остатка от деления в регистр eax. Строка "call iprintLF" вызывает процедуру iprintLF для вывода значения на экран вместе с переводом строки.

## Задание для самостоятельной работы

Создаем новый файл в каталоге

![Создаем файл](image/15.jpg)

Открываем его и заполняем, чтобы решалось выражение (2+x)^2

Компилируем программу и проверяем для x=2 и для x=8

![Проверяем работу программы](image/16.jpg)

# Выводы

Мы приобрели навыки создания исполнительных файлов для решения выражений и освоили арифметические инструкции в NASM.
