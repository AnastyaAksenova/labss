---
## Front matter
lang: ru-RU
title: Structural approach to the deep learning method
author: |
	Leonid A. Sevastianov\inst{1,3}
	\and
	Anton L. Sevastianov\inst{1}
	\and
	Edik A. Ayrjan\inst{2}
	\and
	Anna V. Korolkova\inst{1}
	\and
	Dmitry S. Kulyabov\inst{1,2}
	\and
	Imrikh Pokorny\inst{4}
institute: |
	\inst{1}RUDN University, Moscow, Russian Federation
	\and
	\inst{2}LIT JINR, Dubna, Russian Federation
	\and
	\inst{3}BLTP JINR, Dubna, Russian Federation
	\and
	\inst{4}Technical University of Košice, Košice, Slovakia
date: NEC--2019, 30 September -- 4 October, 2019 Budva, Montenegro

## Formatting
toc: false
slide_level: 2
theme: metropolis
header-includes: 
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
aspectratio: 43
section-titles: true
---

# Лабораторная работа 6
##Поиск файлов. Перенаправление ввода-вывода. Просмотр запущенных процессов
###Аксенова Анастасия

## Цель работы

Ознакомление с инструментами поиска файлов и фильтрации текстовых данных.
Приобретение практических навыков: по управлению процессами (и заданиями), по
проверке использования диска и обслуживанию файловых систем.

##Запись в файл
Записала, в файл file.txt название файлов, содержащийхся в определённом каталоге. Для того, чтобы записать в файл file.txt названия файлов, содержащихся в каталоге /etc, использовала команду «ls–a/etc> file.txt». Далее с помощью команды «ls-a~ >> file.txt» дописываю в этот же файл названия файлов, содержащихся в домашнем каталоге. Командой «catfile.txt» просматриваю файл, чтобы убедиться в правильности действий. (рис. [-@fig:001])

![](61.jpg){ #fig:001 width=70% }

##Редактор gedit
Запускаю редактор gedit в фоновом режиме командой «gedit&». После этого на экране появляется окно редактора.(рис. [-@fig:002])

![](612.jpg){ #fig:002 width=70% }

##Работа с командой gedit
Чтобы определить идентификатор процесса gedit, использую команду «ps| grep-i“gedit”». Из рисунка видно, что наш процесс имеет PID 24249. Узнать идентификатор процесса можно также, используя команду «pgrep gedit»или «pidof gedit».(рис. [-@fig:003])

![](613.jpg){ #fig:003 width=70% }

##Команда kill
Прочитав информацию о команде kill с помощью команды «man kill», использую её для завершения процесса gedit (команда «kill 24249») (рис. [-@fig:004]) (рис. [-@fig:005]) 


![](614.jpg){ #fig:004 width=70% }
![](615.jpg){ #fig:005 width=70% }

##Команды df, du

Выполнила команды df и du, предварительно получив более подробную информацию об этих командах, с помощью команды man. (рис. [-@fig:006]) (рис. [-@fig:007]) (рис. [-@fig:008]) (рис. [-@fig:009]) 

![](616.jpg){ #fig:006 width=70% }
![](617.jpg){ #fig:007 width=70% }
![](618.jpg){ #fig:008 width=70% }
![](619.jpg){ #fig:009 width=70% }

#Вывод
В ходе выполнения данной лабораторной работы я изучила инструменты поиска файлови фильтрации текстовых данных, а также приобрела практические навыки: по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем.


## {.standout}

Спасибо всем спасибо
