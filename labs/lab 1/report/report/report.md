---
## Front matter
title: "Отчёт по лабораторной работе"
subtitle: "Дисциплина: Архитектура ЭВМ"
author: "Перегудов Александр Вадимович"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

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

Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

# Теоретическое введение

# Выполнение лабораторной работы

1. Открыл интрефейс для создания виртаульных машин. (рис. @fig:001)

![Интерфейс.](1.PNG){#fig:001 width=70%}

2. Настроил количество ядер и оперативной памяти. (рис. @fig:002)

![Настройка.](2.PNG){#fig:002 width=70%}

3. Настроил размер диска. (рис. @fig:003)

![Настройка](3.PNG){#fig:003 width=70%}

4. Все параметры. (рис. @fig:004)

![Параметры](4.PNG){#fig:004 width=70%}

5. Настроил очередь загрузки и включил EFI. (рис. @fig:005)

![Настройка](disk_and_gpu.PNG){#fig:005 width=70%}

6. Настроил IDE Controller. (рис. @fig:006)

![Настройка](ide_controller.PNG){#fig:006 width=70%}

7. Настроил систему перетаскивания и общего буфера обмена. (рис. @fig:007)

![Параметры](sda.PNG){#fig:007 width=70%}

8. Сменил графический контроллер на vmsvga и включил 3d ускорение. (рис. @fig:008)

![Параметры](gra.PNG){#fig:008 width=70%}

9. Запустил программу для установки системы. (рис. @fig:009)

![liveinst](5.PNG){#fig:009 width=70%}

10. Выбрал язык. (рис. @fig:010)

![Языки](6.PNG){#fig:010 width=70%}

11. Переместился на интерфейс для определения основных параметров системы. (рис. @fig:011)

![Меню](8.PNG){#fig:011 width=70%}

12. Выбрал диск. (рис. @fig:012)

![Выбранный диск](9.PNG){#fig:012 width=70%}

13. Настроил учётную запись. (рис. @fig:013)

![Параметры](10.PNG){#fig:013 width=70%}

14. Завершил установку. (рис. @fig:014)

![Завершение](7.PNG){#fig:014 width=70%}

15. Обновил все пакеты. (рис. @fig:015)

![Обновление](11.PNG){#fig:015 width=70%}

16. Установил tmux. (рис. @fig:016)

![Установка](13.PNG){#fig:016 width=70%}

17. Отключил систему безопасности SELinux изменив конфиг системы. (рис. @fig:017)

![Конфиг](13.PNG){#fig:017 width=70%}

18. Перезагрузил систему. (рис. @fig:018)

![reboot](reboot_after_driver.PNG){#fig:018 width=70%}

19. Установил группу пакетов Development Tools. (рис. @fig:019)

![Development Tools](dev.PNG){#fig:019 width=70%}

20. Установил dkms. (рис. @fig:020)

![dkms](dkms.PNG){#fig:020 width=70%}

21. Подключил образ диска дополнений гостевой ОС. (рис. @fig:021)

![dkms](guest_os.PNG){#fig:021 width=70%}

22. Подмонтировал диск. (рис. @fig:022)

![Монтирование](mount.PNG){#fig:022 width=70%}

23. Установил драйвера. (рис. @fig:023)

![Установка](driver.PNG){#fig:023 width=70%}

24. Перезагрузил систему. (рис. @fig:024)

![reboot](reboot_after_driver.PNG){#fig:024 width=70%}

25. Создал конфигурационный файл ~/.config/sway/config.d/95-system-keyboard-config.conf. (рис. @fig:025)

![touch](touch.PNG){#fig:025 width=70%}

26. Отредактировал конфигурационный файл 95-system-keyboard-config.conf. (рис. @fig:026)

![Редактированый файл конфига](exec.PNG){#fig:026 width=70%}

27. Отредактировал конфигурационный файл /etc/X11/xorg.conf.d/00-keyboard.conf. (рис. @fig:027)

![Редактированый файл конфига](redacted_keyboard_conf.PNG){#fig:027 width=70%}

28. Перезагрузил систему. (рис. @fig:028)

![reboot](reboot_after_keyboard_conf.PNG){#fig:028 width=70%}

29. Добавил своего пользователя в группу vboxsf. (рис. @fig:029)

![Добавление пользователя](sudo_adding_to_group.PNG){#fig:029 width=70%}

30. В хостовой системе подключил разделяемую папку. (рис. @fig:030)

![Консоль windows](cmd.PNG){#fig:030 width=70%}

31. Скачал pandoc-crossref. (рис. @fig:031)

![Файл на github](crossref.PNG){#fig:031 width=70%}

32. Скачал pandoc соответсвующий pandoc-crossref версии. (рис. @fig:032)

![Файл на github](pandoc.PNG){#fig:032 width=70%}

33. Разархивировал скачанные архивы. (рис. @fig:033)

![Разархивация](unzip.PNG){#fig:033 width=70%}

34. Скопировал файл в /usr/local/bin.

![Копирование pandoc](crossref_copy.PNG){#fig:034 width=70%}
![Копирование pandoc](crossref1_copy.PNG){#fig:035 width=70%}
![Копирование pandoc](pandoc_copy.PNG){#fig:036 width=70%}

35. Установил TeXlive. (рис. @fig:037)

![Установка](texlive.PNG){#fig:037 width=70%}

36. Вывел некоторую информацию о системе.

![Версия ядра Linux](dz1.PNG){#fig:038 width=70%}
![Частота процессора](dz2.PNG){#fig:039 width=70%}
![Модель процессора](dz3.PNG){#fig:040 width=70%}
![Объём доступной оперативной памяти](dz4.PNG){#fig:041 width=70%}
![Тип обнаруженного гипервизора](dz5.PNG){#fig:042 width=70%}
![Тип файловой системы корневого раздела](dz6.PNG){#fig:043 width=70%}
![Последовательность монтирования файловых систем](dz7.PNG){#fig:044 width=70%}

# Выводы

В данной лабораторной работе были усвоены практические навыки установки операционной системы на виртуальную машину и навыки настройки минимально необходимых для дальнейшей работы сервисов.

Какую информацию содержит учётная запись пользователя?
Ответ: имя, группа, пароль, права доступа.

Укажите команды терминала и приведите примеры:

для получения справки по команде
Ответ: man "команда" - man ls

для перемещения по файловой системе
Ответ: cd "название директории" - cd /usr/local

для просмотра содержимого каталога
Ответ: ls

для определения объёма каталога
Ответ: du -sh "название директории" - du -sh /usr/local

для создания / удаления каталогов / файлов
Ответ: mkdir "название директории" - mkdir /usr/local/rrrrrrrss, 
      touch "название файла" - touch random_name
      rm -r "название директории" - rm -r "/usr/local/"
      rm "имя файла" - rm random_name

для задания определённых прав на файл / каталог
Ответ:chmod "разрешения" "файл или директория" - chmod 755 script.sh

для просмотра истории команд.
Ответ: history

Что такое файловая система? Приведите примеры с краткой характеристикой.
Ответ: Файловая система - это способ организации и хранения данных на компьютере или другом устройстве. Она определяет способ, которым файлы и каталоги организуются, и предоставляет интерфейс для доступа к ним. Файловые системы могут различаться по своим характеристикам, таким как поддерживаемые функции, производительность, безопасность и многое другое.

NTFS (New Technology File System):

Операционная система: Windows NT, Windows XP, Windows Vista, Windows 7, Windows 8, Windows 10.
Особенности: Поддержка разрешений NTFS, журналирование для обеспечения целостности данных, поддержка файлов размером до 16 ЭБ.

ext4 (Fourth Extended Filesystem):

Операционная система: Linux.
Особенности: Журналирование для повышения надежности и восстановления данных, поддержка файлов размером до 16 ТБ, поддержка разрешений Unix.

Как посмотреть, какие файловые системы подмонтированы в ОС?
Ответ: mount

Как удалить зависший процесс?
kill "PID процесса"

# Список литературы{.unnumbered}

1. Dash, P. Getting Started with Oracle VM VirtualBox / P. Dash. – Packt Publishing Ltd, 2013. – 86 сс.
2. Colvin, H. VirtualBox: An Ultimate Guide Book on Virtualization with VirtualBox. VirtualBox / H. Colvin. – CreateSpace Independent Publishing Platform, 2015. – 70 сс.
3. Vugt, S. van. Red Hat RHCSA/RHCE 7 cert guide : Red Hat Enterprise Linux 7 (EX200 and EX300) : Certification Guide. Red Hat RHCSA/RHCE 7 cert guide / S. van Vugt. – Pearson IT Certification, 2016. – 1008 сс.
4. Робачевский, А. Операционная система UNIX / А. Робачевский, С. Немнюгин, О. Стесик. – 2-е изд. – Санкт-Петербург : БХВ-Петербург, 2010. – 656 сс.
5. Немет, Э. Unix и Linux: руководство системного администратора. Unix и Linux / Э. Немет, Г. Снайдер, Т.Р. Хейн, Б. Уэйли. – 4-е изд. – Вильямс, 2014. – 1312 сс.
6. Колисниченко, Д.Н. Самоучитель системного администратора Linux : Системный администратор / Д.Н. Колисниченко. – Санкт-Петербург : БХВ-Петербург, 2011. – 544 сс.
7. Robbins, A. Bash Pocket Reference / A. Robbins. – O’Reilly Media, 2016. – 156 сс.