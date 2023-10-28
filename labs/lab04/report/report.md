---
## Front matter
title: "Лабораторная работа №4"
subtitle: "Cоздание и процесс обработки программ на языке ассемблера NASM"
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
Целью работы является освоение процедуры компиляции и сборки программ, написанных на ассемблере NASM.
# Выполнение лабораторной работы
Создадим каталог для работы с программами на языке ассемблера NASM

![Создание каталога](image/1.png)

Перейдём в созданный каталог.

![Открытие созданного каталога](image/2.png)

Создадим текстовый файл с именем hello.asm.

![Создание текстового файла](image/3.png)

Откроем этот файл с помощью текстового редактора gedit и введём в него текст из лабораторной работы.

![Открытие созданного файла и ввод текста](image/4.png)

Для компиляции текста программы «Hello World» необходимо написать:

![Команда для компиляции текста программы](image/5.png)

Проверим работу команды

![Проверка работы команды](image/6.png)

Скомпилируем исходный файл hello.asm в obj.o.

![Компиляция исходного файла](image/7.png)

С помощью команды ls проверим, что файлы были созданы.

![Проверка](image/8.png)

Получим исполняемую программу и объектный файл. Для этого передадим на обработку компоновщику.

![Передача на обработку компановщику](image/9.png)

С помощью команды ls проверим, что исполняемый файл hello был создан.

![Проверка](image/10.png)

Теперь выполним следующую команду:

![Выполнение новой команды](image/11.png)

С помощью команды ls выполним проверку.

![Проверка](image/12.png)

Запустим на выполнение созданный исполняемый файл, находящийся в текущем каталоге.

![Запуск на выполнение созданного исполняемого файла](image/13.png)

В каталоге ~/work/arch-pc/lab04 с помощью команды cp создадим копию файла hello.asm с именем lab4.asm.

![Создание копии файла](image/14.png)

С помощью текстового редактора внесём изменения в текст программы в файле lab4.asm так, чтобы вместо Hello world! на экран выводилась строка с фамилией и именем.

![Изменение текста программы](image/15.png)

Оттранслируем полученный текст программы lab4.asm в объектный файл. Выполним компоновку объектного файла и запустим получившийся исполняемый файл.

![Трансляция текста программы](image/16.png)

# Выводы
В ходе выполнения лабораторной работы мы освоели процедуры компиляции и сборки программ, написанных на ассемблере NASM.
