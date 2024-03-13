---
## Front matter
lang: ru-RU
title: Структура научной презентации
subtitle: Простейший шаблон
author:
  - Шония Ника Гигловна
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 13 июля 2005

## i18n babel
babel-lang: russian
babel-otherlangs: english

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

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Шония Ника Гигловна
  * студентка НММбд-03-23
  * Российский университет дружбы народов
  * <https://github.com/NikaShoniya/study_2023-2024_os-intro.git>

:::
::: {.column width="30%"}

![](./image/ника.jpg)

:::
::::::::::::::

# Вводная часть

## Актуальность

 данный момент существует 2 основных реализации:

    pass — классическая реализация в виде shell-скриптов (https://www.passwordstore.org/);
    gopass — реализация на go с дополнительными интегрированными функциями (https://www.gopass.pw/).

Дальше в тексте будет использоваться программа pass, но всё то же самое можно сделать с помощью программы gopass.

## Объект и предмет исследования



    qtpass
        qtpass — может работать как графический интерфейс к pass, так и как самостоятельная программа. В настройках можно переключаться между использованием pass и gnupg.

    gopass-ui
        gopass-ui — интерфейс к gopass.

    webpass
        Репозиторий: https://github.com/emersion/webpass
        Веб-интерфейс к pass.
        Написано на golang.

## Цели и задачи

Использование chezmoi для управления файлами конфигурации домашнего каталога пользователя.

## Материалы и методы

- Процессор `pandoc` для входного формата Markdown
- Результирующие форматы
	- `pdf`
	- `html`
- Автоматизация процесса создания: `Makefile`

# Создание презентации

## Процессор `pandoc`

- Pandoc: преобразователь текстовых файлов
- Сайт: <https://pandoc.org/>
- Репозиторий: <https://github.com/jgm/pandoc>

## Формат `pdf`

- Использование LaTeX
- Пакет для презентации: [beamer](https://ctan.org/pkg/beamer)
- Тема оформления: `metropolis`

## Код для формата `pdf`

```yaml
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
```

## Формат `html`

- Используется фреймворк [reveal.js](https://revealjs.com/)
- Используется [тема](https://revealjs.com/themes/) `beige`

## Код для формата `html`

- Тема задаётся в файле `Makefile`

```make
REVEALJS_THEME = beige 
```
# Результаты

## Получающиеся форматы

- Полученный `pdf`-файл можно демонстрировать в любой программе просмотра `pdf`
- Полученный `html`-файл содержит в себе все ресурсы: изображения, css, скрипты



