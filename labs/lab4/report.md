---
## Front matter
title: "Лабораторная работа №4."
subtitle: "Основы интерфейса взаимодействия пользователя с системой Unix на уровне командной строки"
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

Приобретение практических навыков взаимодействия пользователя с системой по-
средством командной строки.

# Теоретическое введение

В операционной системе типа Linux взаимодействие пользователя с системой обычно
осуществляется с помощью командной строки посредством построчного ввода ко-
манд. При этом обычно используется командные интерпретаторы языка shell: /bin/sh;
/bin/csh; /bin/ksh.
Формат команды. Командой в операционной системе называется записанный по
специальным правилам текст (возможно с аргументами), представляющий собой ука-
зание на выполнение какой-либо функций (или действий) в операционной системе.
Обычно первым словом идёт имя команды, остальной текст — аргументы или опции,
конкретизирующие действие.
Общий формат команд можно представить следующим образом:
<имя_команды><разделитель><аргументы>.

# Выполнение работы

1. Определим полное имя нашего домашнего каталога. Далее относительно этого ката-
лога будут выполняться последующие упражнения.

![имя домашнего каталога](image/имя_дом_каталога.jpg){#fig:001 width=70%}

2. Перейдем в каталог /tmp..

![каталог tmp](image/каталог_tmp.jpg){#fig:001 width=70%}

3. Выведем на экран содержимое каталога /tmp. Для этого используем команду ls
с различными опциями.

![ls /tmp](image/ls_tmp.jpg){#fig:001 width=70%}

![ls-l /tmp](image/ls-l.jpg){#fig:001 width=70%}

![ls-a /tmp](image/ls-a.jpg){#fig:001 width=70%}

4. Определим, что в каталоге /var/spool нет подкаталога с именем cron.

![cron in spool](image/spool.jpg){#fig:001 width=70%}

5. Перейдем в наш домашний каталог и выведем на экран его содержимое. Опре-
делим, что мы являемся владельцем файлов и подкаталогов.

![владелец каталогов](image/владелец.jpg){#fig:001 width=70%}

6. В домашнем каталоге создадим новый каталог с именем newdir, в каталоге ~/newdir создадим новый каталог с именем morefun.

![newdir and morefun](image/mkdir_more.jpg){#fig:001 width=70%}

7. В домашнем каталоге создадим одной командой три новых каталога с именами
letters, memos, misk. Затем удалим эти каталоги одной командой..

![создание letter, memos, misk](image/mkdir_letters.jpg){#fig:001 width=70%}

![удаление letter, memos, misk](image/rmdir_letters.jpg){#fig:001 width=70%}

8. Удалим ранее созданный каталог ~/newdir командой rm. Проверим,
был ли каталог удалён.

![-r newdir](image/-r_newdir.jpg){#fig:001 width=70%}

9. С помощью команды man определим, какую опцию команды ls нужно использо-
вать для просмотра содержимое не только указанного каталога, но и подкаталогов,
входящих в него.

![-R](image/-R.jpg){#fig:001 width=70%}

10. С помощью команды man определим набор опций команды ls, позволяющий отсорти-
ровать по времени последнего изменения выводимый список содержимого каталога
с развёрнутым описанием файлов.

![сортировка по времени](image/savetime.jpg){#fig:001 width=70%}

11. Используем команду man для просмотра описания опций следующих команд: cd, pwd, mkdir,
rmdir, rm.

![опции cd](image/cd.jpg){#fig:001 width=70%}

![опции pwd](image/pwd.jpg){#fig:001 width=70%}

![опции mkdir](image/mkdir.jpg){#fig:001 width=70%}

![опции rmdir](image/rmdir.jpg){#fig:001 width=70%}

![опции rm](image/rm.jpg){#fig:001 width=70%}

12. Используя информацию, полученную при помощи команды history, выполним мо-
дификацию и исполнение команды из буфера обмена.

![history](image/history.jpg){#fig:001 width=70%}

# Выводы

Я приобрел практические навыки взаимодействия пользователя с системой по-
средством командной строки.

# Список литературы{.unnumbered}

Кулябов Д.С. "Материалы к лабораторным работам"
