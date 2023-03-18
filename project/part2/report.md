---
## Front matter
title: "Индивидуальный проект этап 2"
subtitle: "Добавление к сайту данных о себе"
author: "Александр Андреевич Шуплецов"

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

Добавить к сайту данные о себе.

# Выполнение работы

1. Разместим фотографию владельца сайта.

![добавление фото владельца](image/1.png){#fig:001 width=70%}

2. Разместим краткое описание владельца сайта (Biography).

![размещение краткой биографии владельца сайта](image/2.png){#fig:001 width=70%}

3. Добавим информацию об интересах (Interests).

![добавление информации об интересах](image/3.png){#fig:001 width=70%}

4. Добавим информацию об образовании (Education).

![добавление информации об образовании](image/4.png){#fig:001 width=70%}

5. Сделаем пост по прошедшей неделе.

![добавление поста о прошедшей неделе](image/5.png){#fig:001 width=70%}

6. Добавили пост на выбранную тему "Управление версиями. Git."

![добавление поста на тему по выбору](image/6.png){#fig:001 width=70%}

# Выводы

Я добавил к сайту данные о себе.

# Список литературы{.unnumbered}

Кулябов Д.С. "Материалы к учебному проекту"
