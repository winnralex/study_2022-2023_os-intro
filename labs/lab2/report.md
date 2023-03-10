---
## Front matter
title: "Отчёт по лабораторной работе №2."
subtitle: "Первоначальная настройка Git"
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

Целью данной работы является изучить идеологию и применение средств контроля версий и освоить умения по работе с git.

# Теоретическое введение
Системы контроля версий (Version Control System, VCS) применяются при работе нескольких человек над одним проектом. Обычно основное дерево проекта хранится в локальном или удалённом репозитории, к которому настроен доступ для участников проекта. При внесении изменений в содержание проекта система контроля версий позволяет их фиксировать, совмещать изменения, произведённые разными участниками проекта, производить откат к любой более ранней версии проекта, если это требуется. В классических системах контроля версий используется централизованная модель, предполагающая наличие единого репозитория для хранения файлов. Выполнение большинства функций по управлению версиями осуществляется специальным сервером. Участник проекта (пользователь) перед началом работы посредством определённых команд получает нужную ему версию файлов. После внесения изменений, пользователь размещает новую версию в хранилище. При этом предыдущие версии не удаляются из центрального хранилища и к ним можно вернуться в любой момент. Сервер может сохранять не полную версию изменённых файлов, а производить так называемую дельта-компрессию — сохранять только изменения между последовательными версиями, что позволяет уменьшить объём хранимых данных. Системы контроля версий поддерживают возможность отслеживания и разрешения конфликтов, которые могут возникнуть при работе нескольких человек над одним файлом. Можно объединить (слить) изменения, сделанные разными участниками (автоматически или вручную), вручную выбрать нужную версию, отменить изменения вовсе или заблокировать файлы для изменения. В зависимости от настроек блокировка не позволяет другим пользователям получить рабочую копию или препятствует изменению рабочей копии файла средствами файловой системы ОС, обеспечивая таким образом, привилегированный доступ только одному пользователю, работающему с файлом. Системы контроля версий также могут обеспечивать дополнительные, более гибкие функциональные возможности. Например, они могут поддерживать работу с несколькими версиями одного файла, сохраняя общую историю изменений до точки ветвления версий и собственные истории изменений каждой ветви. Кроме того, обычно доступна информация о том, кто из участников, когда и какие изменения вносил. Обычно такого рода информация хранится в журнале изменений, доступ к которому можно ограничить. В отличие от классических, в распределённых системах контроля версий центральный репозиторий не является обязательным. Среди классических VCS наиболее известны CVS, Subversion, а среди распределённых — Git, Bazaar, Mercurial. Принципы их работы схожи, отличаются они в основном синтаксисом используемых в работе команд.

# Выполнение лабораторной работы

1. Базовая настройка git.

![Базовая настройка git](image/Базовая настройка git.jpg){#fig:001 width=70%}

2. Зададим имя и email владельца репозитория.

![зададим имя и email владельца репозитория](image/зададим имя и email владельца репозитория.jpg){#fig:001 width=70%}

3. Зададим параметр autocrlf и параметр safecrlf.

![зададим параметр autocrlf и параметр safecrlf](image/зададим параметр autocrlf и параметр safecrlf.jpg){#fig:001 width=70%}

4. Настроим utf-8 в выводе сообщений git.

![Настроим utf-8 в выводе сообщений git](image/Настроим utf-8 в выводе сообщений git.jpg){#fig:001 width=70%}

5. Создание ssh ключи.

![Создание ssh ключи](image/Создание ssh ключи.jpg){#fig:001 width=70%}

6. Создание rsa ключа.

![Создание rsa ключа](image/Создание rsa ключа.jpg){#fig:001 width=70%}

7. Добавление PGP ключа в GitHub.

![Добавление PGP ключа в GitHub](image/Добавление PGP ключа в GitHub.jpg){#fig:001 width=70%}

8. Введем фразу пароль для PGP ключа.

![Введем фразу пароль для PGP ключа](image/Введем фразу пароль для PGP ключа.jpg){#fig:001 width=70%}

9. Указываем Git применять его при подписи коммитов.

![указываем Git применять его при подписи коммитов](image/указываем Git применять его при подписи коммитов.jpg){#fig:001 width=70%}

10. Авторизация на GitHub.

![Авторизация](image/Авторизация.jpg){#fig:001 width=70%}

11. Авторизация на GitHub проведена успешно.

![Авторизация на GitHub](image/Авторизация на GitHub.jpg){#fig:001 width=70%}

12. Создание репозитория курса на основе шаблона.

![Сознание репозитория курса на основе шаблона](image/Сознание репозитория курса на основе шаблона.jpg){#fig:001 width=70%}

13. Создание рабочего пространства.

![Создание рабочего пространства](image/Создание рабочего пространства.jpg){#fig:001 width=70%}

14. Настройка каталога курса.

![Настройка каталога курса](image/Настройка каталога курса.jpg){#fig:001 width=70%}

15. Перейдем в каталог курса.

![Перейдем в каталог курса](image/Перейдем в каталог курса.jpg){#fig:001 width=70%}

16. Настроим репозиторий курса.

![Настройка репозитория](image/Настройка репозитория.jpg){#fig:001 width=70%}

# Выводы

Я изучил идеологию и применение средств контроля версий, освоил умения по работе с git.

# Контрольные вопросы

1. Что такое системы контроля версий (VCS) и для решения каких задач они предназначаются? 
Система контроля версий — программное обеспечение для облегчения работы с изменяющейся информацией. Система управления версиями позволяет хранить несколько версий одного и того же документа, при необходимости возвращаться к более ранним версиям, определять, кто и когда сделал то или иное изменение, и многое другое. Системы контроля версий (Version Control System, VCS) применяются для:
• Хранение полной истории изменений 
• причин всех производимых изменений 
• Откат изменений, если что-то пошло не так 
• Поиск причины и ответственного за появления ошибок в программе 
• Совместная работа группы над одним проектом 
• Возможность изменять код, не мешая работе других пользователей 

2. Объясните следующие понятия VCS и их отношения: хранилище, commit, история, рабочая копия. 
Репозиторий - хранилище версий - в нем хранятся все документы вместе с историей их изменения и другой служебной информацией. Commit — отслеживание изменений, сохраняет разницу в изменениях Рабочая копия - копия проекта, связанная с репозиторием (текущее состояние файлов проекта, основанное на версии из хранилища (обычно на последней)) История хранит все изменения в проекте и позволяет при необходимости обратиться к нужным данным. 

3. Что представляют собой и чем отличаются централизованные и децентрализованные VCS? 
Приведите примеры VCS каждого вида. Централизованные VCS (Subversion; CVS; TFS; VAULT; AccuRev): 
• Одно основное хранилище всего проекта 
• Каждый пользователь копирует себе необходимые ему файлы из этого репозитория, изменяет и, затем, добавляет свои изменения обратно Децентрализованные VCS (Git; Mercurial; Bazaar): 
• У каждого пользователя свой вариант (возможно не один) репозитория 
• Присутствует возможность добавлять и забирать изменения из любого репозитория
В классических системах контроля версий используется централизованная модель, предполагающая наличие единого репозитория для хранения файлов. Выполнение большинства функций по управлению версиями осуществляется специальным сервером. В отличие от классических, в распределённых системах контроля версий центральный репозиторий не является обязательным. 

4. Опишите действия с VCS при единоличной работе с хранилищем. 
Сначала создаем и подключаем удаленный репозиторий. Затем по мере изменения проекта отправлять эти изменения на сервер.

5. Опишите порядок работы с общим хранилищем VCS. 
Участник проекта (пользователь) перед началом работы посредством определённых команд получает нужную ему версию файлов. После внесения изменений, пользователь размещает новую версию в хранилище. При этом предыдущие версии не удаляются из центрального хранилища и к ним можно вернуться в любой момент.

6. Каковы основные задачи, решаемые инструментальным средством git? 
Первая — хранить информацию о всех изменениях в вашем коде, начиная с самой первой строчки, а вторая — обеспечение удобства командной работы над кодом. 

7. Назовите и дайте краткую характеристику командам git. 
Наиболее часто используемые команды git: 
• создание основного дерева репозитория: git init 
• получение обновлений
(изменений) текущего дерева из центрального репозитория: git pull 
• отправка всех произведённых изменений локального дерева в центральный репозиторий: git push 
• просмотр списка изменённых файлов в текущей директории: git status 
• просмотр текущих изменения: git diff 
• сохранение текущих изменений: – добавить все изменённые и/или созданные файлы и/или каталоги: git add. – добавить конкретные изменённые и/или созданные файлы и/или каталоги: git add имена_файлов 
• удалить файл и/или каталог из индекса репозитория (при этом файл и/или каталог остаётся в локальной директории): git rm имена_файлов 
• сохранение добавленных изменений: – сохранить все добавленные изменения и все изменённые файлы: git commit -am 'Описание коммита' – сохранить добавленные изменения с внесением комментария через встроенный редактор git commit 
• создание новой ветки, базирующейся на текущей: git checkout -b имя_ветки 
• переключение на некоторую ветку: git checkout
имя_ветки (при переключении на ветку, которой ещё нет в локальном репозитории, она будет создана и связана с удалённой) • отправка изменений конкретной ветки в центральный репозиторий: git push origin имя_ветки • слияние ветки с текущим деревом: git merge —no-ff имя_ветки 
• удаление ветки: – удаление локальной уже слитой с основным деревом ветки: git branch -d имя_ветки – принудительное удаление локальной ветки: git branch -D имя_ветки – удаление ветки с центрального репозитория: git push origin :имя_ветки 

8. Приведите примеры использования при работе с локальным и удалённым репозиториями. git push –all (push origin master любой branch) 

9. Что такое и зачем могут быть нужны ветви (branches)? 
Ветвление («ветка», branch) — один из параллельных участков истории в одном хранилище, исходящих из одной версии (точки ветвления). 
• Обычно есть главная ветка (master), или ствол (trunk).
• Между ветками, то есть их концами, возможно слияние. Используются для разработки новых функций.

10. Как и зачем можно игнорировать некоторые файлы при commit? 
Во время работы над проектом так или иначе могут создаваться файлы, которые не требуется добавлять в последствии в репозиторий. Например, временные файлы, создаваемые редакторами, или объектные файлы, создаваемые компиляторами. Можно прописать шаблоны игнорируемых при добавлении в репозиторий типов файлов в файл .gitignore с помощью сервисов.

# Список литературы{.unnumbered}

Кулябов Д.С. "Материалы к лабораторной работе"
