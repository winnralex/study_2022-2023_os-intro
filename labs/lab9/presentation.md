---
## Front matter
lang: ru-RU
title: Лабораторная работа №9
subtitle: Текстовый редактор emacs
author:
  - Шуплецов А. А.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 8 апреля 2023

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

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором emacs.

## Выполнение работы

## Установим и откроем emacs.

![открытие emacs](image/1.png){#fig:001 width=70%}

## Cоздадим файл lab07.sh с помощью комбинации Ctrl-x Ctrl-f (C-x C-f).

![создание файла lab07.sh](image/2.png){#fig:001 width=70%}

## Наберем текст, данный в материалах к лабораторным работам.

![набор текста в emacs](image/3.png){#fig:001 width=70%}

## Cохраним файл с помощью комбинации Ctrl-x Ctrl-s (C-x C-s).

![сохранение файла в emacs](image/4.png){#fig:001 width=70%}

## Проделаем с текстом стандартные процедуры редактирования, каждое действие осуществим комбинацией клавиш: 

Вырежем одной командой целую строку (С-k). Вставим эту строку в конец файла (C-y). Выделим область текста (C-space).Скопируем область в буфер обмена (M-w). Вставим область в конец файла.Вновь выделим эту область и на этот раз вырежем её (C-w). Отменим последнее действие (C-/).

![редактирование текста с помощью комбинаций клавиш](image/5.png){#fig:001 width=70%}

## Выведем список активных буферов на экран (C-x C-b).

![вывод списка активных буферов на экран](image/7.png){#fig:001 width=70%}

## Поделим фрейм на 4 части: разделим фрейм на два окна по вертикали (C-x 3), а затем каждое из этих окон на две части по горизонтали (C-x 2).

![разделение фрейма на 4 части](image/8.png){#fig:001 width=70%}

## Переключимся в режим поиска (C-s) и найдем несколько слов, присутствующих в тексте.

![поиск через C-s](image/9.1.png){#fig:001 width=70%}

## Перейдем в режим поиска и замены (M-%), введем текст, который следует найти и заменить, нажмем Enter , затем введем текст для замены. После того как будут подсвечены результаты поиска, нажмем ! для подтверждения замены.

![режим поиска и замены](image/9.4.png){#fig:001 width=70%}

## Попробуем другой режим поиска, нажав M-s o.

![поиск через M-s o](image/9.5.png){#fig:001 width=70%}

## Вывод

Я познакомился с операционной системой Linux, получил практические навыки работы с редактором emacs.

## Список литературы

Кулябов Д.С. "Материалы к лабораторным работам"
