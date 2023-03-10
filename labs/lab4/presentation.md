---
## Front matter
lang: ru-RU
title: Лабораторная работа №4
subtitle: Основы интерфейса взаимодействия пользователя с системой Unix на уровне командной строки.
author:
  - Шуплецов А. А.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 4 марта 2023

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

Приобретение практических навыков взаимодействия пользователя с системой по-
средством командной строки.

## Выполнение работы

## Определим полное имя нашего домашнего каталога. Далее относительно этого каталога будут выполняться последующие упражнения.

![имя домашнего каталога](image/имя_дом_каталога.jpg){#fig:001 width=70%}

## Перейдем в каталог /tmp..

![каталог tmp](image/каталог_tmp.jpg){#fig:001 width=70%}

## Выведем на экран содержимое каталога /tmp. Для этого используем команду ls с различными опциями.

![ls /tmp](image/ls_tmp.jpg){#fig:001 width=70%}

![ls-l /tmp](image/ls-l.jpg){#fig:001 width=70%}

![ls-a /tmp](image/ls-a.jpg){#fig:001 width=70%}

## Перейдем в наш домашний каталог и выведем на экран его содержимое. Определим, что мы являемся владельцем файлов и подкаталогов.

![владелец каталогов](image/владелец.jpg){#fig:001 width=70%}

## В домашнем каталоге создадим новый каталог с именем newdir, в каталоге ~/newdir создадим новый каталог с именем morefun.

![newdir and morefun](image/mkdir_more.jpg){#fig:001 width=70%}

## В домашнем каталоге создадим одной командой три новых каталога с именами letters, memos, misk. Затем удалим эти каталоги одной командой.

![создание letter, memos, misk](image/mkdir_letters.jpg){#fig:001 width=70%}

![удаление letter, memos, misk](image/rmdir_letters.jpg){#fig:001 width=70%}

## Удалим ранее созданный каталог ~/newdir командой rm. Проверим, был ли каталог удалён.

![-r newdir](image/-r_newdir.jpg){#fig:001 width=70%}

## С помощью команды man определим, какую опцию команды ls нужно использовать для просмотра содержимое не только указанного каталога, но и подкаталогов входящих в него.

![-R](image/-R.jpg){#fig:001 width=70%}

## С помощью команды man определим набор опций команды ls, позволяющий отсортировать по времени последнего изменения выводимый список содержимого каталога с развёрнутым описанием файлов.

![сортировка по времени](image/savetime.jpg){#fig:001 width=70%}

## Используем команду man для просмотра описания опций следующих команд: cd, pwd, mkdir, rmdir, rm.

![опции cd](image/cd.jpg){#fig:001 width=70%}

![опции pwd](image/pwd.jpg){#fig:001 width=70%}

![опции mkdir](image/mkdir.jpg){#fig:001 width=70%}

![опции rmdir](image/rmdir.jpg){#fig:001 width=70%}

![опции rm](image/rm.jpg){#fig:001 width=70%}

## Используя информацию, полученную при помощи команды history, выполним модификацию и исполнение команды из буфера обмена.

![history](image/history.jpg){#fig:001 width=70%}

## Вывод

Я приобрел практические навыки взаимодействия пользователя с системой по-
средством командной строки.

## Список литературы

Кулябов Д.С. "Материалы к лабораторным работам"
