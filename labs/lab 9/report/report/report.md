---
## Front matter
title: "Лабораторная работа № 9"
subtitle: "Операционные системы"
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
  Options:
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
## Misc Options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---


# Цель работы

Освоение основных возможностей командной оболочки Midnight Commander. Приобретение навыков практической работы по просмотру каталогов и файлов; манипуляций с ними.

# Задание

# Теоретическое введение

Здесь описываются теоретические аспекты, связанные с выполнением работы.

Например, в табл. [-@tbl:std-dir] приведено краткое описание стандартных каталогов Unix.

: Описание некоторых каталогов файловой системы GNU Linux {#tbl:std-dir}

| Имя каталога | Описание каталога                                                                                                          |
|--------------|----------------------------------------------------------------------------------------------------------------------------|
| `/`          | Корневая директория, содержащая всю файловую                                                                               |
| `/bin `      | Основные системные утилиты, необходимые как в однопользовательском режиме, так и при обычной работе всем пользователям     |
| `/etc`       | Общесистемные конфигурационные файлы и файлы конфигурации установленных программ                                           |
| `/home`      | Содержит домашние директории пользователей, которые, в свою очередь, содержат персональные настройки и данные пользователя |
| `/media`     | Точки монтирования для сменных носителей                                                                                   |
| `/root`      | Домашняя директория пользователя  `root`                                                                                   |
| `/tmp`       | Временные файлы                                                                                                            |
| `/usr`       | Вторичная иерархия для данных пользователя                                                                                 |

Более подробно про Unix см. в [@tanenbaum_book_modern-os_ru; @robbins_book_bash_en; @zarrelli_book_mastering-bash_en; @newham_book_learning-bash_en].

# Выполнение лабораторной работы

Открыл справку Midnight Commander (рис. [-@fig:001], [-@fig:002]).

![Команда](image/1.PNG){#fig:001 width=70%}

![Справка Midnight Commander](image/2.PNG){#fig:002 width=70%}

Запустил Midnight Commander (рис. [-@fig:099], [-@fig:003]).

![Команда](image/0.PNG){#fig:099 width=70%}

![Midnight Commander](image/3.PNG){#fig:003 width=70%}

Создал файл file.txt (рис. [-@fig:004], [-@fig:005]).

![Команда](image/4.PNG){#fig:004 width=70%}

![Созданный файл](image/5.PNG){#fig:005 width=70%}

Отредактировал файл file.txt (рис. [-@fig:006]).

![Отредактированный файл](image/6.PNG){#fig:006 width=70%}

Скопировал файл file.txt как файл file2.txt (рис. [-@fig:007], [-@fig:008]).

![Меню копирования](image/7.PNG){#fig:007 width=70%}

![Скопированный файл](image/8.PNG){#fig:008 width=70%}

Отредактировал файл file2.txt (рис. [-@fig:009]).

![Отредактированный файл](image/9.PNG){#fig:009 width=70%}

Скопировал файл file2.txt как файл file3.txt в папку Download (рис. [-@fig:010], [-@fig:011]).

![Меню перемещения](image/10.PNG){#fig:010 width=70%}

![Перемещённый файл](image/11.PNG){#fig:011 width=70%}

Отредактировал файл file3.txt (рис. [-@fig:012]).

![Отредактированный файл](image/12.PNG){#fig:012 width=70%}

Открыл подменю file и использовал опцию chown для одной директории и одного файла (рис. [-@fig:013], [-@fig:014], [-@fig:015]).

![Подменю file](image/13.PNG){#fig:013 width=70%}

![Информация о папке](image/14.PNG){#fig:014 width=70%}

![Информация о файле](image/15.PNG){#fig:015 width=70%}

Открыл подменю Left (рис. [-@fig:016]).

![Подменю Left](image/16.PNG){#fig:016 width=70%}

Использовал опции Quick view, Info, Tree (рис. [-@fig:017] [-@fig:018], [-@fig:019]).

![Quick view](image/17.PNG){#fig:017 width=70%}

![Info](image/18.PNG){#fig:018 width=70%}

![Tree](image/19.PNG){#fig:019 width=70%}

Открыл подменю file и использовал опцию View (рис. [-@fig:020], [-@fig:021]).

![Подменю file](image/20.PNG){#fig:020 width=70%}

![Файл file.txt](image/21.PNG){#fig:021 width=70%}

Открыл подменю file и использовал опцию Edit  (рис. [-@fig:022], [-@fig:023]).

![Подменю file](image/22.PNG){#fig:022 width=70%}

![Отредактированный файл file.txt](image/23.PNG){#fig:023 width=70%}

Вышел из редактора без сохранения (рис. [-@fig:024]).

![Меню закрытия файла](image/24.PNG){#fig:024 width=70%}

Открыл подменю file и использовал опцию Mkdir и создал директорию test (рис. [-@fig:025], [-@fig:026]).

![Подменю file](image/25.PNG){#fig:025 width=70%}

![Меню создания директории](image/26.PNG){#fig:026 width=70%}

Скопировал файл file.txt в папку test (рис. [-@fig:027]).

![Меню копирования](image/27.PNG){#fig:027 width=70%}

Открыл подменю Command и использовал опцию Find file (рис. [-@fig:028]).

![Подменю Command](image/28.PNG){#fig:028 width=70%}

Открыл подменю Command и нашёл файлы по определённым критериям (рис. [-@fig:029], [-@fig:030]).

![Меню опции Find file](image/29.PNG){#fig:029 width=70%}

![Результаты нахождения](image/30.PNG){#fig:030 width=70%}

Удалил файл file.txt (рис. [-@fig:032]).

![Подтверждение удаления](image/32.PNG){#fig:032 width=70%}

Открыл подменю Command и использовал опцию Command history (рис. [-@fig:031],  [-@fig:033]).

![Подменю Command](image/31.PNG){#fig:031 width=70%}

![Команда touch после использования history](image/33.PNG){#fig:033 width=70%}

Использовал touch при помощи команды history (рис. [-@fig:034]).

![Команда](image/34.PNG){#fig:034 width=70%}

Открыл подменю Command и выключил панели для ввода команды (рис. [-@fig:035]).

![Подменю Command](image/35.PNG){#fig:035 width=70%}

Ввёл команду для cd ~ для перехода в домашний каталог (рис. [-@fig:036]).

![Команда](image/36.PNG){#fig:036 width=70%}

Открыл подменю Command (рис. [-@fig:037]).

![Подменю Command](image/37.PNG){#fig:037 width=70%}

Открыл файл меню (рис. [-@fig:038]).

![Файл меню](image/38.PNG){#fig:038 width=70%}

Открыл файл расширений (рис. [-@fig:039]).

![Файл расширений](image/39.PNG){#fig:039 width=70%}

Открыл подменю Options (рис. [-@fig:040]).

![Подменю Options](image/40.PNG){#fig:040 width=70%}

Изменил некоторые опции в меню Layout (рис. [-@fig:041]).

![Меню Layout](image/41.PNG){#fig:041 width=70%}

Изменил некоторые опции в меню Panel options (рис. [-@fig:042]).

![Меню Panel Options](image/42.PNG){#fig:042 width=70%}

Изменил некоторые опции в меню Confirmation (рис. [-@fig:043]).

![Меню Confirmation](image/43.PNG){#fig:043 width=70%}

Создал файл file.txt (рис. [-@fig:044]).

![Команда](image/44.PNG){#fig:044 width=70%}

Скопировал текст из случайного файла в файл file.txt (рис. [-@fig:045]).

![Созданный файл](image/45.PNG){#fig:045 width=70%}

Открыл файл file.txt (рис. [-@fig:046]).

![Файл file.txt](image/46.PNG){#fig:046 width=70%}

Отредактировал файл и сохранил его (рис. [-@fig:047]).

![Отредактированный файл](image/47.PNG){#fig:047 width=70%}

Открыл файл с исходным текстом на c++ (рис. [-@fig:048]).

![Файл c++](image/48.PNG){#fig:048 width=70%}

Выключил подсветку синтаксиса для c++ (рис. [-@fig:049], [-@fig:050]).

![Меню Command](image/49.PNG){#fig:049 width=70%}

![Файл c++ без подстветки синтаксиса](image/50.PNG){#fig:050 width=70%}

# Выводы

Освоение основных возможностей командной оболочки Midnight Commander. Приобретение навыков практической работы по просмотру каталогов и файлов; манипуляций с ними.

Были освоены основные возможности командной оболочки Midnight Commander. Также были приобретенны навыки практической работы по просмотру каталогов, файлов и манипуляций с ними.

# Список литературы{.unnumbered}

::: {#refs}
:::
