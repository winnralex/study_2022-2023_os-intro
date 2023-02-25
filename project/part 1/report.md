---
## Front matter
title: "Индивидуальный проект этап 1."
subtitle: "Размещение на Github pages заготовки для персонального сайта."
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

Разместить на Github pages заготовки для персонального сайта.

# Задание


- Установить необходимое программное обеспечение.
- Скачать шаблон темы сайта.
- Разместить его на хостинге git.
- Установить параметр для URLs сайта.
- Разместить заготовку сайта на Github pages.

# Выполнение работы

1. Установим нужную версию HUGO.

![установка HUGO](image/установка_HUGO.jpg){#fig:001 width=70%}

2. Сделаем репозиторий по шаблону.

![шаблон репозиторий](image/шаблон_репозиторий.jpg){#fig:001 width=70%}

3. Создадим локальный сайт.

![локальный сайт](image/локальный_сайт.jpg){#fig:001 width=70%}

4. Создаем свой репозиторий.

![свой репозиторий](image/свой_репозиторий.jpg){#fig:001 width=70%}

5. Отправим файлы на Git.

![отправка_на_GIT](image/отправка_на_GIT.jpg){#fig:001 width=70%}

6. Открываем созданный нами сайт.

![сайт](image/сайт.jpg){#fig:001 width=70%}

# Выводы

Я разместил на Github pages заготовки для персонального сайта.

# Список литературы{.unnumbered}

Кулябов Д.С. "Материалы к учебному проекту"
