---
## Front matter
lang: ru-RU
title: Лабораторная работа №5
subtitle: Анализ файловой системы Linux. Команды для работы с файлами и каталогами.
author:
  - Шуплецов А. А.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 7 марта 2023

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

  * Шуплецов Александр Андреевич
  * студент ФФМиЕН
  * Российский университет дружбы народов
  * https://github.com/winnralex

## Цели и задачи

Ознакомление с файловой системой Linux, её структурой, именами и содержанием каталогов. Приобретение практических навыков по применению команд для работы с файлами и каталогами, по управлению процессами (и работами), по проверке использования диска и обслуживанию файловой системы.

## Выполнение работы

## Выполним все примеры, приведённые в первой части описания лабораторной работы. 

## Примеры с cp.
![примеры с cp](image/cp.jpg){#fig:001 width=70%}

## Примеры с mv.
![примеры с mv](image/mv.jpg){#fig:001 width=70%}

## Примеры с chmod.
![примеры с chmod](image/chmod.jpg){#fig:001 width=70%}

## Скопируем файл /usr/include/sys/io.h в домашний каталог и назовем его equipment. 

![назвали equipment](image/2.1.jpg){#fig:001 width=70%}

## В домашнем каталоге создадим директорию ~/ski.places.  

![создали ski.places](image/2.2.jpg){#fig:001 width=70%}

## Переместим файл equipment в каталог ~/ski.places.  

![переместиили equipment](image/2.3.jpg){#fig:001 width=70%}

## Переименуем файл ~/ski.plaсes/equipment в ~/ski.plaсes/equiplist. 

![переименовали equipment](image/2.4.jpg){#fig:001 width=70%}

## Создадим в домашнем каталоге файл abc1 и скопируйте его в каталог ~/ski.plaсes, назовем его equiplist2. 

![создали файл abc1](image/2.5.jpg){#fig:001 width=70%}

## Cоздадим каталог с именем equipment в каталоге ~/ski.plaсes, переместим файлы ~/ski.plaсes/equiplist и equiplist2 в каталог ~/ski.plaсes/equipment 

![переместили файлы в equipment](image/2.7.jpg){#fig:001 width=70%}

## Создадим и переместим каталог ~/newdir в каталог ~/ski.plaсes и назовем его plans. 

![создали plans](image/2.8.jpg){#fig:001 width=70%}

## Определим опции команды chmod, необходимые для того, чтобы присвоить выделенные права доступа, считая, что в начале таких прав нет.

![определили опции chmod](image/3.jpg){#fig:001 width=70%}

## Просмотрим содержимое файла /etc/password, скопируем файл ~/feathers в файл ~/file.old. 

![копирование feathers](image/4.2.jpg){#fig:001 width=70%}

## Переместим файл ~/file.old в каталог ~/play.  

![переместили файл file.old ](image/4.3.jpg){#fig:001 width=70%}

## Скопируем каталог ~/play в каталог ~/fun. 

![скопировали каталог play в fun](image/4.4.jpg){#fig:001 width=70%}

## Переместим каталог ~/fun в каталог ~/play и назовем его games.  

![переместили fun](image/4.5.jpg){#fig:001 width=70%}

## Лишим владельца файла ~/feathers права на чтение. 

![лишили права на чтение](image/4.6.jpg){#fig:001 width=70%}

## Убедимся, что у нас нет прав просмотреть или скопировать файл feathers. 

![действия с feathers](image/4.7.jpg){#fig:001 width=70%}

## Дадим владельцу файла ~/feathers право на чтение.

![дали право на чтение](image/4.9.jpg){#fig:001 width=70%}

## Лишим владельца каталога ~/play права на выполнение, перейдем в каталог ~/play и убедимся, что у нас нет прав на это действие. 

![лишили права на выполнение](image/4.10.jpg){#fig:001 width=70%}

## Дадим владельцу каталога ~/play право на выполнение. 

![дали право на выполнение](image/4.12.jpg){#fig:001 width=70%}

## Введем man по командам mount, fsck, mkfs, kill и узнаем подробную информацию об этих командах. 

## Информация о mount.

![информация mount](image/mount.jpg){#fig:001 width=70%}

## Информация о fsck.

![информация fsck](image/fsck.jpg){#fig:001 width=70%}

## Информация о mkfs.

![информация mkfs](image/mkfs.jpg){#fig:001 width=70%}

## Информация о kill.

![информация kill](image/kill.jpg){#fig:001 width=70%}

## Вывод

Я ознакомился с файловой системой Linux, её структурой, именами и содержанием каталогов, приобрел практические навыки по применению команд для работы с файлами и каталогами, по управлению процессами (и работами), по проверке использования диска и обслуживанию файловой системы.

## Список литературы

Кулябов Д.С. "Материалы к лабораторным работам"
