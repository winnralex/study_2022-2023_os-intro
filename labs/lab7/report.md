---
## Front matter
title: "Лабораторная работа №7."
subtitle: "Командная оболочка Midnight Commander."
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

Освоение основных возможностей командной оболочки Midnight Commander. Приобретение навыков практической работы по просмотру каталогов и файлов; манипуляций с ними.

# Теоретическое введение

Панель в mc отображает список файлов текущего каталога. Абсолютный путь к этому каталогу отображается в заголовке панели. У активной панели заголовок и одна из еёстрок подсвечиваются. Управление панелями осуществляется с помощью определённых комбинаций клавиш или пунктов меню mc. Панели можно поменять местами. Для этого и используется комбинация клавиш Ctrl-u или команда меню mc Переставить панели . Также можно временно убрать отображение панелей (отключить их) с помощью комбинации клавиш Ctrl-o или команды меню mc Отключить панели . Это может быть полезно, например, если необходимо увидеть вывод какой-то информации на экран после выполнения какой-либо команды shell. С помощью последовательного применения комбинации клавиш Ctrl-x d есть возможность сравнения каталогов, отображённых на двух панелях. Панели могут дополнительно быть переведены в один из двух режимов: Информация или Дерево. В режиме Информация на панель выводятся сведения о файле и текущей файловой системе, расположенных на активной панели. В режиме Дерево на одной из панелей выводится структура дерева каталогов. Управлять режимами отображения панелей можно через пункты меню mc Правая панель и Левая панель.

# Выполнение работы

1. Изучим информацию о mc, вызвав в командной строке man mc.

![man mc](image/1.png){#fig:001 width=70%}

2. Запустим из командной строки mc, изучим его структуру и меню.

![запуск mc](image/2.png){#fig:001 width=70%}

3. Используя возможности подменю Файл , выполним:

– просмотр содержимого текстового файла

![просмотр содержимого текстового файла](image/5.1.png){#fig:001 width=70%}

– редактирование содержимого текстового файла (без сохранения результатов
редактирования)

![редактирование содержимого текстового файла](image/5.2.png){#fig:001 width=70%}

- создание каталога

![создание каталога](image/5.3.png){#fig:001 width=70%}

– копирование файлов в созданный каталог

![копирование файлов в созданный каталог](image/5.4.png){#fig:001 width=70%}

4. С помощью соответствующих средств подменю Команда осуществим:

– поиск в файловой системе файла с заданными условиями

![поиск в файловой системе](image/6.1.png){#fig:001 width=70%}

– выбор и повторение предыдущей команды

![выбор и повторение предыдущей команды](image/6.2.png){#fig:001 width=70%}

- анализ файла меню и файла расширений

![анализ файла меню](image/6.4.1.png){#fig:001 width=70%}

![анали файла расширений](image/6.4.2.png){#fig:001 width=70%}

5. Вызовем подменю Настройки. Освоим операции, определяющие структуру экрана mc
(Full screen, Double Width, Show Hidden Files и т.д.). 

![вызов подменю Настройки](image/7.png){#fig:001 width=70%}

6. Создадим текстовой файл text.txt

![создание текстового файла text.txt](image/8.png){#fig:001 width=70%}

7. Откроем этот файл с помощью встроенного в mc редактора, вставим в открытый файл небольшой фрагмент текста, скопированный из Интернета.

![открытие текстового файла text.txt](image/9.png){#fig:001 width=70%}

8. Поработаем с текстовым файлом text.txt и сохраним изменения в нем. 

![сохранение изменений в файле text.txt](image/10.png){#fig:001 width=70%}

9. Откроем файл с исходным текстом на языке программирования C++.

![открытие файла cpp](image/11.png){#fig:001 width=70%}

10. Используя меню редактора, выключим подстветку синтаксиса.

![выключение подсветки синтаксиса в файле cpp](image/12.png){#fig:001 width=70%}

# Выводы

Я освоил основные возможности командной оболочки Midnight Commander, приобрел навыки практической работы по просмотру каталогов и файлов, манипуляций с ними.

# Список литературы{.unnumbered}

Кулябов Д.С. "Материалы к лабораторным работам"
