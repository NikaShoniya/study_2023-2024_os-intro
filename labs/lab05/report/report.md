---
## Front matter
title: "Лабораторная работа №5"
subtitle: "Операционные системы"
author: "Шония Ника Гигловна"

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

Научиться работать с шаблонами и шрифтами

# Задание

1. Менеджер паролей pass
2. Управление файлами конфигурации

# Теоретическое введение


    Шаблоны используются для изменения содержимого файла в зависимости от среды.
    Используется синтаксис шаблонов Go.
    Файл интерпретируется как шаблон, если выполняется одно из следующих условий:
        имя файла имеет суффикс .tmpl;
        файл находится в каталоге .chezmoitemplates.

Данные шаблона

    Полный список переменных шаблона:

    chezmoi data

    Источники переменных:
        файлы .chezmoi, например, .chezmoi.os;
        файлы конфигурации .chezmoidata.$FORMAT. Форматы (json, jsonc, toml, yaml) читаются в алфавитном порядке;
        раздел data конфигурационного файла.

# Выполнение лабораторной работы

1. Менеджер паролей pass
Установка pass ![Установка команды pass](image/01.png){#fig:001 width=70%}
Установка gopass ![gopass](image/02.png){#fig:001 width=70%}
Инициализация хранилища ![Инициализация хранилища](image/03.png){#fig:001 width=70%}
Создала репозиторий ![репозиторий](image/04.png){#fig:001 width=70%}
Создадим структуру git ![Создадим структуру git](image/05.png){#fig:001 width=70%}
задать адрес репозитория на хостинге ![задать адрес репозитория на хостинге ](image/06.png){#fig:001 width=70%}
Для синхронизации выполняется следующая команда ![git pull](image/07.png){#fig:001 width=70%}
![git push](image/08.png){#fig:001 width=70%}
необходимо вручную закоммитить и выложить изменения ![необходимо вручную закоммитить и выложить изменения](image/09.png){#fig:001 width=70%}
Проверить статус синхронизации модно командой ![Проверить статус синхронизации модно командой](image/10.png){#fig:001 width=70%}
кроме плагина к броузеру устанавливается программа, обеспечивающая интерфейс native messaging ![кроме плагина к броузеру устанавливается программа, обеспечивающая интерфейс native messaging](image/11.png){#fig:001 width=70%}
![.](image/12.png){#fig:001 width=70%}
Добавить новый пароль ![Добавить новый пароль](image/13.png){#fig:001 width=70%}
2. Управление файлами конфигурации
Установить дополнительное программное обеспечение ![Установить дополнительное программное обеспечение](image/14.png){#fig:001 width=70%}(image/15.png){#fig:001 width=70%}
Установка бинарного файла ![Установка бинарного файла](image/16.png){#fig:001 width=70%}
Создадим свой репозиторий для конфигурационных файлов на основе шаблона ![.](image/17.png){#fig:001 width=70%}
Инициализируйте chezmoi с вашим репозиторием dotfiles ![Инициализируйте chezmoi с вашим репозиторием dotfiles](image/19.png){#fig:001 width=70%}
Проверьте, какие изменения внесёт chezmoi в домашний каталог, запустив chezmoi diff ![chezmoi diff](image/20.png){#fig:001 width=70%}
На второй машине инициализируйте chezmoi с вашим репозиторием dotfiles ![На второй машине инициализируйте chezmoi с вашим репозиторием dotfiles](image/21.png){#fig:001 width=70%}
Разные действия с командой chezmoi ![chezmoi](image/22.png){#fig:001 width=70%}
При существующем каталоге chezmoi можно получить и применить последние изменения из вашего репозитория ![.](image/23.png){#fig:001 width=70%}
Выполнение команд ![Выполнение команд](image/24.png){#fig:001 width=70%}

# Выводы

Скачали шрифты, сделали работу с шаблонами

# Список литературы{.unnumbered}

::: {#refs}
:::
