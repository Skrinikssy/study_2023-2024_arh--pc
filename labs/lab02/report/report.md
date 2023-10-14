---
## Front matter
title: "Лабораторная работа №2"
subtitle: "Система контроля версий GIT"
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
Целью работы является приобретение практических навыков по
работе в системе git.
# Выполнение лабораторной работы
1.Создание учетное записи на github.com

![Базовая настройка git.](image/1.jpg)

Создаем предварительную конфигурацию git.

![Настроим utf-8в выводе сообщений git.](image/2.jpg)

![Зададим имя начальной ветки (назовём ее master)](image/3.jpg)

![Параметр autocrlf](image/4.jpg)

![Параметр safecrlf](image/5.jpg)

![Создание SSH-ключа](image/6.jpg)

![Создали ssh-ключ](image/7.jpg)

![Подтверждение ключа на GIT](image/8.jpg)

![Подтверждение ключа на GIT 2](image/9.jpg)

Создание рабочего пространства и репозитория курса на основе
шаблона.
Откройте терминал и создайте каталог для предмета “Архитектура
компьютера”

![Создали каталог](image/10.jpg)

Создание репозитория курса на основе шаблона.
Репозиторий на основе шаблона можно создать через web-интерфейс
github.
Перейдем на страницу репозитория с шаблонами курса
https://github.com/yamadharma/cour se-
directory-student-template. Далее выберите use
this template

![Создали репозиторий по шаблону](image/11.jpg)

В открывшемся окне задайте имя репозитория (Repository
name) study_2023–2024_arhpc и создайте репозиторий
(кнопка Create repository from template). Откройте
терминал и перейдите в каталог курса:

![Клонируем созданный репозиторий](image/12.jpg)

![Настройка каталога курса](image/13.jpg)

![Перейдем в каталог курса](image/14.jpg)

![Удалим лишние файлы](image/15.jpg)

![Создадим необходимые каталоги](image/16.jpg)

![Создадим необходимые каталоги](image/17.jpg)

![Отправим файлы на сервер](image/18.jpg)

![Отправим файлы на сервер](image/19.jpg)

# Выводы
В ходе выполнения лабораторной работы мы приобрели практические навыки по работе в системе git.
