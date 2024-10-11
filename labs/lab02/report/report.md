---
## Front matter
title: "Лабораторная работа №2
subtitle: "дисциплина: Архитектура компьютера"
author: "Гаврилейко Алина Александровна"

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

Целью работы является изучить идеологию и применение системы контроля
версий. Приобрести практические навыки по работе с системой git

# Задание

На основе методических указаний провести работу с базовыми командами
системы контроля версий git, выучить применение команд для разных случаев
использования, настроить GitHub.

# Теоретическое введение

Системы контроля версий (Version Control System, VCS) применяются при
работе нескольких человек над одним проектом. Обычно основное дерево проекта
хранится в локальном или удалённом репозитории, к которому настроен доступ для
участников проекта. При внесении изменений в содержание проекта система контроля
версий позволяет их фиксировать, совмещать изменения, произведённые разными
участниками проекта, производить откат к любой более ранней версии проекта, если
это
требуется.
В
классических
системах
контроля
версий
используется
централизованная модель, предполагающая наличие единого репозитория для
хранения файлов. Выполнение большинства функций по управлению версиями
осуществляется специальным сервером. Участник проекта (пользователь) перед
началом работы посредством определённых команд получает нужную ему версию
файлов. После внесения изменений, пользователь размещает новую версию в
хранилище. При этом предыдущие версии не удаляются из центрального хранилища и
к ним можно вернуться в любой момент. Сервер может сохранять не полную версию
изменённых файлов, а производить так называемую дельта-компрессию — сохранять
только изменения между последовательными версиями, что позволяет уменьшить
объём хранимых данных. Системы контроля версий поддерживают возможность
отслеживания и разрешения конфликтов, которые могут возникнуть при работе
нескольких человек над одним файлом. Можно объединить (слить) изменения,
сделанные разными участниками (автоматически или вручную), вручную выбрать
нужную версию, отменить изменения вовсе или заблокировать файлы для изменения.
В зависимости от настроек блокировка не позволяет другим пользователям получить
рабочую копию или препятствует изменению рабочей копии файла средствами
файловой системы ОС, обеспечивая таким образом, привилегированный доступ
только одному пользователю, работающему с файлом.

# Выполнение лабораторной работы

## Настройка GitHub

Создаю учетную запись на сайте GitHub, заполняю данные учетной записи и создаю аккаунт (рис. [-@fig:001]).

![Создание аккаунта на GitHub](image/placeimg_800_600_tech.jpg){#fig:001 width=70%}

Открываю виртуальную машину, затем терминал и делаю предварительную конфигурацию Git. Вбиваю команду git config –global user.name ‘’, указываю свое имя и фамилию (рис. [-@fig:002]).

![Предварительная конфигурация Git](image/placeimg_800_600_tech.jpg){#fig:002 width=70%}
 
затем пишу команду git config –global user.email ‘’, указываю почту владельца. (рис. [-@fig:003]).

![Предварительная конфигурация Git](image/placeimg_800_600_tech.jpg){#fig:003 width=70%}

Настраиваю utf-8 в выводе сообщений git для корректного отображения символов
























































# Выводы

Здесь кратко описываются итоги проделанной работы.

# Список литературы{.unnumbered}

::: {#refs}
:::
