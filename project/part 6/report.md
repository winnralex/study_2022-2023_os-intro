---
## Front matter
title: "Индивидуальный проект этап 6"
subtitle: "Размещение двуязычного сайта на Github"
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

Разместить двуязычный сайт на Github.

# Выполнение работы

1. Сделаем поддержку английского и русского языков.

![поддержка двух языков](image/1.png){#fig:001 width=70%}

2. Разместим элементы сайта на обоих языках.

![элементы сайта на двух языках](image/2.png){#fig:001 width=70%}

3. Разместим контент на обоих языках.

![контент на обоих языках](image/3.png){#fig:001 width=70%}

4. Сделаем пост по прошедшей неделе.

![пост по прошедшей неделе](image/4.png){#fig:001 width=70%}

5. Добавим пост на тему по выбору: "Устойчивое развитие".

![пост на тему "Устойчивое развитие"](image/5.png){#fig:001 width=70%}

# Выводы

Я разместил двуязычный сайт на Github.

# Список литературы{.unnumbered}

Кулябов Д.С. "Материалы к учебному проекту"
