---
## Front matter
title: "Лабораторная работа 4"
subtitle: "Основы интерфейса взаимодействия пользователя с системой Unix на уровне командной строки"
author: "Аксенова Анастасия"


# Цель работы

приобретение практических навыков взаимодействия пользователя с системой посредством командной строки.
 
# Задание

1. Определите полное имя вашего домашнего каталога. Далее относительно этого каталога будут выполняться последующие упражнения.
2. Выполните следующие действия:
2.1. Перейдите в каталог /tmp.
2.2. Выведите на экран содержимое каталога /tmp. Для этого используйте команду ls
с различными опциями. Поясните разницу в выводимой на экран информации.
2.3. Определите, есть ли в каталоге /var/spool подкаталог с именем cron?
2.4. Перейдите в Ваш домашний каталог и выведите на экран его содержимое. Определите, кто является владельцем файлов и подкаталогов?
3. Выполните следующие действия:
3.1. В домашнем каталоге создайте новый каталог с именем newdir.
3.2. В каталоге ~/newdir создайте новый каталог с именем morefun.
3.3. В домашнем каталоге создайте одной командой три новых каталога с именами
letters, memos, misk. Затем удалите эти каталоги одной командой.
3.4. Попробуйте удалить ранее созданный каталог ~/newdir командой rm. Проверьте,
был ли каталог удалён.
3.5. Удалите каталог ~/newdir/morefun из домашнего каталога. Проверьте, был ли
каталог удалён.
4. С помощью команды man определите, какую опцию команды ls нужно использовать для просмотра содержимое не только указанного каталога, но и подкаталогов,
входящих в него.
5. С помощью команды man определите набор опций команды ls, позволяющий отсортировать по времени последнего изменения выводимый список содержимого каталога
с развёрнутым описанием файлов.
6. Используйте команду man для просмотра описания следующих команд: cd, pwd, mkdir,
rmdir, rm. Поясните основные опции этих команд.
7. Используя информацию, полученную при помощи команды history, выполните модификацию и исполнение нескольких команд из буфера команд.


# Выполнение лабораторной работы

1. Определим полное имя моего домашнего каталога. Далее относительно этого каталога будут выполняться последующие упражнения.

![](1.jpg){ #fig:001 width=70% }

2. Выполняем следующие действия: 
    • 2.1. Переходим в каталог /tmp. 
    • 2.2. Выводим на экран содержимое каталога /tmp. 

![](2.jpg){ #fig:002 width=70% }

2.3. Определяем, есть ли в каталоге /var/spool подкаталог с именем cron. (Данный каталог я не обнаружила, но если бы он был, мы бы без проблем проверили существование подкаталога с пом-ю команды ls)

![](3.jpg){ #fig:003 width=70% }

 2.4. Переходим в мой домашний каталог и выводим на экран его содержимое. Определяем, кто является его владельцем с помощью команды ls -l.
 
 ![](44.jpg){ #fig:004 width=70% }
 ![](5.jpg){ #fig:005 width=70% }
 
 3. Выполняем следующие действия: (их я делала дома в онлайн консоли, поэтому они выглядят странно)
    • 3.1. В домашнем каталоге создаем новый каталог с именем newdir. 
   
![](6.jpg){ #fig:006 width=70% }

    • 3.2. В каталоге ~/newdir создаем новый каталог с именем morefun. 
    
![](7.jpg){ #fig:007 width=70% }

    • 3.3. В домашнем каталоге создаем одной командой три новых каталога с именами letters, memos, misk. Затем удаляем эти каталоги одной командой.
    
![](8.jpg){ #fig:008 width=70% }
![](9.jpg){ #fig:009 width=70% }

    • 3.4. Попробуем удалить ранее созданный каталог ~/newdir командой rm. (Удален он не был, потому что данная команда удаляет файлы а не каталоги)
    
 ![](10.jpg){ #fig:010 width=70% }
 
    • 3.5. Удаляем каталог ~/newdir/morefun из домашнего каталога. 
    
 ![](11.jpg){ #fig:011 width=70% }
 
 4. С помощью команды man определяем, какую опцию команды ls нужно использовать для просмотра содержимое не только указанного каталога, но и подкаталогов, входящих в него. Нужно использовать  опцию (-R).
 
![](12.jpg){ #fig:012 width=70% }

5. С помощью команды man определите набор опций команды ls, позволяющий отсортировать по времени последнего изменения выводимый список содержимого каталога с развёрнутым описанием файлов. Опция  (-c -l)

![](13.jpg){ #fig:013 width=70% }

6. Используем команду man для просмотра описания следующих команд: cd, pwd, mkdir, rmdir, rm. Поясним основные опции этих команд на примере команды pwd:
Опишем опции команды 
-L или --logical
Не разыменовывать символические ссылки. Если путь содержит символические ссылки, то выводить их без преобразования в исходный путь.

-P или --physical

Преобразовывать символические ссылки в исходные имена. Если путь содержит символические ссылки, то они будут преобразованы в названия исходных директорий, на которые они указывают.

--help
Показать справку по команде pwd.

--version
Показать версию утилиты pwd.

7. Используя информацию, полученную при помощи команды history, выполняем модификацию и исполнение нескольких команд из буфера команд. (Данная команда служит для просмотра последних действий, например, мы хотим посмотреть последние 5 действий…)

![](14.jpg){ #fig:014 width=70% }


# Выводы

мы приобрели некоторые практические навыки взаимодействия пользователя с системой посредством командной строки.



