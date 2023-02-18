---
## Front matter
title: "Отчет по лабораторной работе №1"
subtitle: "Установка OC Linux"
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

Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.
# Теоретическое введение

Fedora (с англ. — «федора», ранее — Fedora Core) — дистрибутив Linux, разрабатываемый Проектом Fedora, спонсируемый компаниями Red Hat и IBM и содержащий возможности, которые в будущем предполагаются к использованию в дистрибутиве Red Hat Enterprise Linux. Цель проекта — построение целостной операционной системы из свободного программного обеспечения силами сообщества в духе экосистемы Red Hat Linux. Версии выходят каждые 6—8 месяцев по публичному расписанию.
VirtualBox (Oracle VM VirtualBox) — программный продукт виртуализации для операционных систем Windows, Linux, FreeBSD[8], macOS, Solaris/OpenSolaris, ReactOS, DOS и других

# Выполнение лабораторной работы

1. Создаем новую виртуальную операционную систему, называем ее Fedora.

![photo_5442968542363371072_x](image/photo_5442968542363371072_x.jpg){#fig:001 width=70%}

2. Задаем параметры ОЗУ и количество виртуальных процессоров.

![photo_5442968542363371073_x](image/photo_5442968542363371073_x.jpg){#fig:001 width=70%}
3. Создаем новый виртуальный жесткий диск.

![photo_5442968542363371075_x](image/photo_5442968542363371075_x.jpg){#fig:001 width=70%}

4. Выбираем установить Fedora на жесткий диск.

![photo_5442968542363371076_x](image/photo_5442968542363371076_x.jpg){#fig:001 width=70%}

5. Выбираем устройство для установки операционной системы.

![photo_5442968542363371077_x](image/photo_5442968542363371077_x.jpg){#fig:001 width=70%}

6. Устанавливаем имя пользователя.

![photo_5442968542363371078_x](image/photo_5442968542363371078_y.jpg){#fig:001 width=70%}

7. Обновляем систему до последней версии.

![photo_5442968542363371079_x](image/photo_5442968542363371079_x.jpg){#fig:001 width=70%}

8. Выставляем автоматические обновления системы.

![photo_5442968542363371081_x](image/photo_5442968542363371081_x.jpg){#fig:001 width=70%}

9. Отключаем SELinux.

![photo_5442968542363371082_x](image/photo_5442968542363371082_x.jpg){#fig:001 width=70%}

![photo_5442968542363371083_x](image/photo_5442968542363371083_x.jpg){#fig:001 width=70%}

10. Устанавливаем необходимые для комфортной работы терминала дополнения.

![photo_5442968542363371085_x](image/photo_5442968542363371085_x.jpg){#fig:001 width=70%}

11. Меняем раскладку клавиатуры.

![photo_5442968542363371086_x](image/photo_5442968542363371086_x.jpg){#fig:001 width=70%}

12. Меняем имя хоста согласно соглашению о наименовании.

![photo_5442968542363371084_x](image/photo_5442968542363371084_x.jpg){#fig:001 width=70%}

13. Устанавливаем pandoc.

![photo_5442968542363371088_x](image/photo_5442968542363371088_x.jpg){#fig:001 width=70%}

14. Устанавливаем texlive.

![photo_5442968542363371087_x](image/photo_5442968542363371087_x.jpg){#fig:001 width=70%}

![photo_5442968542363371089_x](image/photo_5442968542363371089_x.jpg){#fig:001 width=70%}

![photo_5442968542363371090_x](image/photo_5442968542363371090_x.jpg){#fig:001 width=70%}


# Домашние задание

1. Получите следующую информацию:

    Версия ядра Linux (Linux version).
    
![photo_5442968542363371091_x](image/photo_5442968542363371091_x.jpg){#fig:001 width=70%}

    Частота процессора (Detected Mhz processor).
    
![photo_5442968542363371092_x](image/photo_5442968542363371092_x.jpg){#fig:001 width=70%}
    Модель процессора (CPU0).
    
![photo_5442968542363371092_x](image/photo_5442968542363371092_x.jpg){#fig:001 width=70%}

    Объём доступной оперативной памяти (Memory available).
    
![photo_5442968542363371094_x](image/photo_5442968542363371094_x.jpg){#fig:001 width=70%}

    Тип обнаруженного гипервизора (Hypervisor detected).
    
![photo_5445220342177055186_x](image/photo_5445220342177055186_x.jpg){#fig:001 width=70%}

    Тип файловой системы корневого раздела.
    
![photo_5445220342177055187_x](image/photo_5445220342177055187_x.jpg){#fig:001 width=70%}

    Последовательность монтирования файловых систем.
    
![photo_5445220342177055188_x](image/photo_5445220342177055188_x.jpg){#fig:001 width=70%}

# Контрольные вопросы


    1. Какую информацию содержит учётная запись пользователя?
    Имя пользователя, пароль, id номер пользователя, id номер основной группы пользователя, домашний каталог пользователя, командный интерпретатор пользователя.

    2. Укажите команды терминала и приведите примеры:
        для получения справки по команде: man
        для перемещения по файловой системе: cd
        для просмотра содержимого каталога: ls
        для определения объёма каталога: du
        для создания / удаления каталогов / файлов: mkdir, rm, -r
        для задания определённых прав на файл / каталог: chmod + x
        для просмотра истории команд history

    3. Что такое файловая система? Приведите примеры с краткой характеристикой.
    Файловая система – это инструмент, позволяющий операционной системе и программам обращаться к нужным файлам и работать с ними. При этом программы оперируют только названием файла, его размером и датой созданий. Все остальные функции по поиску необходимого файла в хранилище и работе с ним берет на себя файловая система накопителя. Пример - FAT – одна из старейших файловых систем, которая была разработана еще в 1977 году программистами компании Microsoft для гибких дисков. Пример - NTFS, или новая технология файловой системы была создана, чтоб устранить недостатки FAT32.
    4. Как посмотреть, какие файловые системы подмонтированы в ОС?
    С помощью команды mount.ls
    5. Как удалить зависший процесс?
    С помощью команды kill.


# Выводы

Я приобрел практические навыки установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

