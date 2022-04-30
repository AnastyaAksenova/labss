---
## Front matter
title: "отчет по лабораторной работе 2"
subtitle: "Управление версиями"
author: "Аксенова Анастасия"

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
Цель данной лабораторной работы -изучить идеологию и применение средств контроля версий. – Освоить умения по работе с git.
# Задание

- Создать базовую конфигурацию для работы с git. 
- Создать ключ SSH. 
- Создать ключ PGP.
– Настроить подписи git.
– Зарегистрироваться на Github.
– Создать локальный каталог для выполнения заданий по предмету.
# Теоретическое введение
Система контроля версий Git представляет собой набор программ командной строки.
Доступ к ним можно получить из терминала посредством ввода команды git с различными опциями.Благодаря тому, что Git является распределённой системой контроля версий, резервную
копию локального хранилища можно сделать простым копированием или архивацией.

# Выполнение лабораторной работы

##Ход работы
###1. Работа с локальным репозиторием
Создадим локальный репозиторий. Сначала сделаем предварительную конфигурацию, указав имя и email владельца репозитория. 
![Создание локального репозитория](image/1.png){ #fig:001 width=70% }

и настроив utf-8 в выводе сообщений git:
![](image/2.png){ #fig:002 width=70% }

Для инициализации локального репозитория, расположенного, например, в каталоге ~/tutorial, введемв командной строке:
![](image/3.png){ #fig:003 width=70% }

После это в каталоге tutorial появится каталог .git, в котором будет храниться история изменений. Создадим тестовый текстовый файл hello.txt и добавим его в локальный репозиторий:
![](image/4.png){ #fig:004 width=70% }

Воспользуемся командой status для просмотра изменений в рабочем каталоге, сделанных с момента последней ревизии:
![Просмотр изменений в рабочем каталоге](image/5.png){ #fig:005 width=70% }

###2. Создаем ключи ssh
– по алгоритму rsa с ключём размером 4096 бит:
– по алгоритму ed25519:
![](image/6.png){ #fig:006 width=70% }
![](image/7.png){ #fig:007 width=70% }
![](image/8.png){ #fig:008 width=70% }

###3. Создаем ключи pgp
– Генерируем ключ
– Из предложенных опций выбираем: – тип RSA and RSA; – размер 4096; – выберите срок действия; значение по умолчанию— 0 (срок действия не истекает никогда). – GPG запросит личную информацию, которая сохранится в ключе: – Имя (не менее 5 символов). – Адрес электронной почты. – При вводе email убедитесь, что он соответствует адресу, используемому на GitHub. – Комментарий. Можно ввести что угодно или нажать клавишу ввода, чтобы оставить это поле пустым
![](image/9.png){ #fig:009 width=70% }
![Ключи ssh и png](image/10.png){ #fig:010 width=70% }

###4. Создание репозитория курса на основе шаблона
–Создаем шаблон рабочего пространства.
– Для 2021–2022 учебного года и предмета «Операционные системы» (код предмета os-intro) создание репозитория примет следующий вид:
![](image/11.png){ #fig:011 width=70% }

###5. Настройка каталога курса
– Перейдем в каталог курса: 32 Лабораторная работа № 2. Управление версиями 1 cd ~/work/study/2021-2022/"Операционные системы"/os-intro.
– Удаляем лишние файлы: 1 rm package.json –
 Создайем необходимые каталоги: 1 make COURSE=os-intro 
– Отправляем файлы на сервер:
![](image/12.png){ #fig:012 width=70% }
![](image/13.png){ #fig:013 width=70% }




# Выводы
мы освоили умения по работе с git.

