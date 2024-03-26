---
## Front matter
lang: ru-RU
title: Лабораторная работа № 8
subtitle: Операционные системы
author:
  - Перегудов А.В.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 30 марта 2024

## i18n babel
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

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

# Информация

## Докладчик

  * Перегудов Александр Вадимович
  * Студент группы НКАбд-04-23
  * Российский университет дружбы народов
  * [1132239659@pfur.ru]
  * <https://github.com/magister6239/study_2023-2024_os-intro>

# Вводная часть

Поиск файлов. Перенаправление ввода-вывода. Просмотр запущенных процессов

## Актуальность

- Умение использовать инструменты поиска файлов является ключевым навыком.
- Перенаправление ввода-вывода используется для множества задач, включая перенаправление вывода команды в файл, чтение ввода из файла вместо стандартного потока ввода и т. д. Это необходимо как для повседневных задач, так и для автоматизации и сценариев оболочки.
- Мониторинг и управление процессами - важная задача для администраторов систем и разработчиков. Знание того, как работать с процессами позволит выполнять более широкий спектр задач и облегчить работу с системой.

## Объект и предмет исследования

- концепция конвеера
- концепция потоков
- find
- grep
- df
- du
- ps
- kill

## Цели и задачи

Получение навыков поиска файлов, управления процессами и работы с потоками ввода-вывода.

## Материалы и методы

- Процессор `pandoc` для входного формата Markdown
- Результирующие форматы
	- `pdf`
	- `html`
- Автоматизация процесса создания: `Makefile`

## Вход в систему

![](image/1.PNG){width=70%}

## Запись в файл file.txt 

![](image/2.PNG){width=70%}

## Запись в файл file.txt

![](image/3.PNG){width=70%}

## Вывод файла file.txt

![](image/4.PNG){width=70%}

## Вывод всех файлов с расширением .conf

![](image/5-1.PNG){width=70%}

## Запись файлов с расширением .conf в файл conf.txt

![](image/5-2.PNG){width=70%}

## Файлы на "c" 

![](image/6.PNG){width=70%}

## Файлы на "h"

![](image/7.PNG){width=70%}

![](image/8.PNG){width=70%}

## Запуск фонового процесса

![](image/9.PNG){width=70%}

![](image/10.PNG){width=70%}

![](image/11.PNG){width=70%}

## Удаление файла logfile

![](image/12.PNG){width=70%}

## Запуск gedit в фоновом режиме

![](image/13.PNG){width=70%}

## Определение pid процесса gedit

![](image/14.PNG){width=70%}

![](image/15.PNG){width=70%}

## Вызов справки kill

![](image/16.PNG){width=70%}

![](image/17.PNG){width=70%}

## Завершение процесса

![](image/18.PNG){width=70%}

## Команда df

![](image/19.PNG){width=70%}

![](image/20.PNG){width=70%}

![](image/21.PNG){width=70%}

## Команда du

![](image/22.PNG){width=70%}

![](image/23.PNG){width=70%}

![](image/24.PNG){width=70%}

## Вывод всех директорий домашнего каталога

![](image/25.PNG){width=70%}

![](image/26.PNG){width=70%}

![](image/27.PNG){width=70%}
