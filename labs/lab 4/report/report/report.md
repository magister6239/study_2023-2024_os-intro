---
## Front matter
title: "Шаблон отчёта по лабораторной работе"
subtitle: "Простейший вариант"
author: "Перегудов Александр Вадимович"

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

Получение навыков правильной работы с репозиториями git.

# Задание

Здесь приводится описание задания в соответствии с рекомендациями
методического пособия и выданным вариантом.

# Теоретическое введение

# Выполнение лабораторной работы

Установка git-flow. (рис. @fig:001)

![Установка git-flow](image/1.JPG){#fig:001 width=70%}

Установка git-flow. (рис. @fig:002)

![Установка git-flow](image/2.JPG){#fig:002 width=70%}

Установка Node.js. (рис. @fig:003)

![Установка Node.js](image/3.JPG){#fig:003 width=70%}

Установка Node.js. (рис. @fig:004)

![Установка Node.js](image/4.JPG){#fig:004 width=70%}

Настройка Node.js. (рис. @fig:005)

![Настройка Node.js](image/5.JPG){#fig:005 width=70%}

Настройка Node.js. (рис. @fig:006)

![Настройка Node.js](image/6.JPG){#fig:006 width=70%}

Создал каталог и перешёл в него. (рис. @fig:007)

![commitizen](image/7.JPG){#fig:007 width=70%}

commitizen. (рис. @fig:008)

![standard-changelog](image/8.JPG){#fig:008 width=70%}

standard-changelog. (рис. @fig:009)

![Создание репозитория git](image/9.JPG){#fig:009 width=70%}

Создание репозитория git. (рис. @fig:010)

![Конфигурация для пакетов Node.js](image/10.JPG){#fig:010 width=70%}

Конфигурация для пакетов Node.js. (рис. @fig:011)

![Сконфигурил формат коммитов](image/11.JPG){#fig:011 width=70%}

Сконфигурил формат коммитов. (рис. @fig:012)

![](image/12.JPG){#fig:013 width=70%}

. (рис. @fig:014)

![](image/13.JPG){#fig:014 width=70%}

. (рис. @fig:015)

![](image/14.JPG){#fig:015 width=70%}

. (рис. @fig:016)

![](image/15.JPG){#fig:016 width=70%}

. (рис. @fig:017)

![](image/16.JPG){#fig:017 width=70%}

. (рис. @fig:018)

![](image/17.JPG){#fig:018 width=70%}

. (рис. @fig:019)

![](image/18.JPG){#fig:019 width=70%}

. (рис. @fig:020)

![](image/19.JPG){#fig:020 width=70%}

. (рис. @fig:021)

![](image/20.JPG){#fig:021 width=70%}

. (рис. @fig:022)

![](image/21.JPG){#fig:022 width=70%}

. (рис. @fig:023)

![](image/22.JPG){#fig:023 width=70%}

. (рис. @fig:024)

![](image/23.JPG){#fig:024 width=70%}

. (рис. @fig:025)

![](image/24.JPG){#fig:025 width=70%}

. (рис. @fig:026)

![](image/25.JPG){#fig:026 width=70%}

. (рис. @fig:027)

![](image/26.JPG){#fig:027 width=70%}


# Выводы

Были получены навыки правильной работы с репозиториями git.

# Список литературы{.unnumbered}

::: {#refs}
:::
