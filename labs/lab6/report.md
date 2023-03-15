---
## Front matter
title: "Лабораторная работа №6."
subtitle: "Поиск файлов. Перенаправление ввода-вывода. Просмотр запущенных процессов."
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

Ознакомление с инструментами поиска файлов и фильтрации текстовых данных.Приобретение практических навыков: по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем.

# Теоретическое введение

В системе по умолчанию открыто три специальных потока:
– stdin — стандартный поток ввода (по умолчанию: клавиатура), файловый дескриптор
0;
– stdout — стандартный поток вывода (по умолчанию: консоль), файловый дескриптор
1;
– stderr — стандартный поток вывод сообщений об ошибках (по умолчанию: консоль),
файловый дескриптор 2.
Большинство используемых в консоли команд и программ записывают результаты своей работы в стандартный поток вывода stdout. Например, команда ls выводит в стандартный поток вывода (консоль) список файлов в текущей директории. Потоки вывода и ввода можно перенаправлять на другие файлы или устройства. Проще всего это делается с помощью символов >, >>, <, <<. Конвейер (pipe) служит для объединения простых команд или утилит в цепочки, в которых результат работы предыдущей команды передаётся последующей. Чаще всего скрипты на Bash используются в качестве автоматизации каких-то рутинных операций в консоли, отсюда иногда возникает необходимость в обработке stdout одной команды и передача на stdin другой команде, при этом результат выполнения команды должен обработан.

# Выполнение работы

1. Осуществим вход в систему, используя соответствующее имя пользователя. 

![вход в систему](image/1.jpg){#fig:001 width=70%}

2. Запишим в файл file.txt названия файлов, содержащихся в каталоге /etc. Допишим в этот же файл названия файлов, содержащихся в нашем домашнем каталоге. 

![запись названий файлов в file.txt](image/2.jpg){#fig:001 width=70%}

3. Выведим имена всех файлов из file.txt, имеющих расширение .conf, после чего
запишим их в новый текстовой файл conf.txt. 

![вывод имен всех файлов из file.txt](image/3.1.jpg){#fig:001 width=70%}

![запись имен файлов в conf.txt](image/3.1.jpg){#fig:001 width=70%}

4. Определим, какие файлы в вашем домашнем каталоге имеют имена, начинавшиеся
с символа c. 

![определение с помощью find](image/4find.jpg){#fig:001 width=70%}

![определение с помощью grep](image/4grep.jpg){#fig:001 width=70%}

5. Выведем на экран (по странично) имена файлов из каталога /etc, начинающиеся
с символа h. 

![вывод имен с h](image/5.jpg){#fig:001 width=70%}

6. Запустим в фоновом режиме процесс, который будет записывать в файл ~/logfile
файлы, имена которых начинаются с log.

![процесс с log](image/6.jpg){#fig:001 width=70%}

7. Удалим файл ~/logfile.

![удаление logfile](image/7.jpg){#fig:001 width=70%}

8. Запустим из консоли в фоновом режиме редактор gedit.. 

![запуск из консоли gedit](image/8.jpg){#fig:001 width=70%}

9. Определим идентификатор процесса gedit, используя команду ps, конвейер и фильтр
grep.

![определение идентификатора процесса gedit](image/9grep.jpg){#fig:001 width=70%}

10. Прочтем справку (man) команды kill, после чего используем её для завершения
процесса gedit. 

![использование kill](image/10.jpg){#fig:001 width=70%}

11. Выполним команды df и du, предварительно получив более подробную информацию
об этих командах, с помощью команды man. 

![выполнение команды df](image/11df.jpg){#fig:001 width=70%}

![выполнение команды du](image/11du.jpg){#fig:001 width=70%}

12. Воспользовавшись справкой команды find, выведим имена всех директорий, имею-
щихся в нашем домашнем каталоге. 

![вывод имен всех директорий](image/12.jpg){#fig:001 width=70%}

# Выводы

Я ознакомился с инструментами поиска файлов и фильтрации текстовых данных, приобрел практические навыки: по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем.

# Список литературы{.unnumbered}

Кулябов Д.С. "Материалы к лабораторным работам"
