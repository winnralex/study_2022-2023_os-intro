---
## Front matter
title: "Лабораторная работа №5."
subtitle: "Анализ файловой системы Linux. Команды для работы с файлами и каталогами."
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

Ознакомление с файловой системой Linux, её структурой, именами и содержанием
каталогов. Приобретение практических навыков по применению команд для работы
с файлами и каталогами, по управлению процессами (и работами), по проверке исполь-
зования диска и обслуживанию файловой системы.

# Теоретическое введение

Для создания текстового файла можно использовать команду touch. Для просмотра файлов небольшого размера можно использовать команду cat. Команда tail выводит умолчанию 10 последних строк файла. Команда cp используется для копирования файлов и каталогов. Команды mv и mvdir предназначены для перемещения и переименования файлов
и каталогов. Каждый файл или каталог имеет права доступа.
В сведениях о файле или каталоге указываются:
– тип файла (символ (-) обозначает файл, а символ (d) — каталог);
– права для владельца файла (r — разрешено чтение, w — разрешена запись, x — разре-
шено выполнение, - — право доступа отсутствует);
– права для членов группы (r — разрешено чтение, w — разрешена запись, x — разрешено
выполнение, - — право доступа отсутствует);
– права для всех остальных (r — разрешено чтение, w — разрешена запись, x — разрешено
выполнение, - — право доступа отсутствует).
 Права доступа к файлу или каталогу можно изменить, воспользовавшись командой
chmod. Сделать это может владелец файла (или каталога) или пользователь с правами
администратора. Режим (в формате команды) имеет следующие компоненты структуры и способ запи-
си:
= установить право
- лишить права
+ дать право
r чтение
w запись
x выполнение
u (user) владелец файла
g (group) группа, к которой принадлежит владелец файла
o (others) все остальные
В работе с правами доступа можно использовать их цифровую запись (восьмеричное
значение) вместо символьной.
Файловая система в Linux состоит из фалов и каталогов. Каждому физическому носи-
телю соответствует своя файловая система.
Существует несколько типов файловых систем. Перечислим наиболее часто встречаю-
щиеся типы:
– ext2fs (second extended filesystem);
– ext2fs (third extended file system);
– ext4 (fourth extended file system);
– ReiserFS;
– xfs;
– fat (file allocation table);
– ntfs (new technology file system).
Для просмотра используемых в операционной системе файловых систем можно вос-
пользоваться командой mount без параметров.

# Выполнение работы

1. Выполним все примеры, приведённые в первой части описания лабораторной работы. 

![примеры с cp](image/cp.jpg){#fig:001 width=70%}

![примеры с mv](image/mv.jpg){#fig:001 width=70%}

![примеры с chmod](image/chmod.jpg){#fig:001 width=70%}

2. Скопируем файл /usr/include/sys/io.h в домашний каталог и назовем его
equipment. 

![назвали equipment](image/2.1.jpg){#fig:001 width=70%}

3. В домашнем каталоге создадим директорию ~/ski.places.  

![создали ski.places](image/2.2.jpg){#fig:001 width=70%}

4. Переместим файл equipment в каталог ~/ski.places.  

![переместиили equipment](image/2.3.jpg){#fig:001 width=70%}

5. Переименуем файл ~/ski.plaсes/equipment в ~/ski.plaсes/equiplist. 

![переименовали equipment](image/2.4.jpg){#fig:001 width=70%}

6. Создадим в домашнем каталоге файл abc1 и скопируйте его в каталог
~/ski.plaсes, назовите его equiplist2. 

![создали файл abc1](image/2.5.jpg){#fig:001 width=70%}

7. Cоздадим каталог с именем equipment в каталоге ~/ski.plaсes, переместим файлы ~/ski.plaсes/equiplist и equiplist2 в каталог ~/ski.plaсes/equipment 

![переместили файлы в equipment](image/2.7.jpg){#fig:001 width=70%}

8. Создадим и переместим каталог ~/newdir в каталог ~/ski.plaсes и назовем
его plans. 

![создали plans](image/2.8.jpg){#fig:001 width=70%}

9. Определим опции команды chmod, необходимые для того, чтобы присвоить перечис-
ленным ниже файлам выделенные права доступа, считая, что в начале таких прав
нет:
drwxr--r-- ... australia
drwx--x--x ... play
-r-xr--r-- ... my_os
-rw-rw-r-- ... feathers 

![определили опции chmod](image/3.jpg){#fig:001 width=70%}

10. Просмотрим содержимое файла /etc/password, скопируем файл ~/feathers в файл ~/file.old. 

![копирование feathers](image/4.2.jpg){#fig:001 width=70%}

11. Переместим файл ~/file.old в каталог ~/play.  

![переместили файл file.old ](image/4.3.jpg){#fig:001 width=70%}

12. Скопируем каталог ~/play в каталог ~/fun. 

![скопировали каталог play в fun](image/4.4.jpg){#fig:001 width=70%}

13. Переместим каталог ~/fun в каталог ~/play и назовем его games.  

![переместили fun](image/4.5.jpg){#fig:001 width=70%}

14. Лишим владельца файла ~/feathers права на чтение. 

![лишили права на чтение](image/4.6.jpg){#fig:001 width=70%}

15. Убедимся, что у нас нет прав просмотреть или скопировать файл feathers. 

![действия с feathers](image/4.7.jpg){#fig:001 width=70%}

16. Дадим владельцу файла ~/feathers право на чтение.

![дали право на чтение](image/4.9.jpg){#fig:001 width=70%}

17. Лишим владельца каталога ~/play права на выполнение, перейдем в каталог ~/play и убедимся, что у нас нет прав на это действие. 

![лишили права на выполнение](image/4.10.jpg){#fig:001 width=70%}

18. Дадим владельцу каталога ~/play право на выполнение. 

![дали право на выполнение](image/4.12.jpg){#fig:001 width=70%}

19. Введем man по командам mount, fsck, mkfs, kill и узнаем подробную информацию об этих командах. 

![информация mount ](image/mount.jpg){#fig:001 width=70%}

![информация fsck ](image/fsck.jpg){#fig:001 width=70%}

![информация mkfs](image/mkfs.jpg){#fig:001 width=70%}

![информация kill ](image/kill.jpg){#fig:001 width=70%}

# Выводы

Мы ознакомились с файловой системой Linux, её структурой, именами и содержанием
каталогов, приобрели практические навыки по применению команд для работы
с файлами и каталогами, по управлению процессами (и работами), по проверке исполь-
зования диска и обслуживанию файловой системы.

# Список литературы{.unnumbered}

Кулябов Д.С. "Материалы к лабораторным работам"
