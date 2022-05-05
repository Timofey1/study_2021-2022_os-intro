---
# Front matter
lang: ru-RU
title: "Индивидуальный проект. Этап 2"
subtitle: "Редактирование информации о себе. И создание поста."
author: "Бешкуров Тимофей Борисович"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---


# Цель работы

Добавить к сайту данные о себе. Добавить пост на тему: "Управление версиями. Git."

# Выполнение лабораторной работы

1. Список добавляемых данных.
- Разместить фотографию владельца сайта.
- Разместить краткое описание владельца сайта (Biography).
- Добавить информацию об интересах (Interests).
- Добавить информацию от образовании (Education).

Для того чтобы изменить данные о себе необходимо зайти в файл `content/authors/admin/_index.md` и изменить там необходимые данные о себе (рис. 1). Также в папку `content/authors/admin/` необходимо положить свою фотографию и назвать её `avatar.jpg` (рис. 2)

![Изменение данных о себе](images/2.png){ #fig:001 width=90% }

![Фотография](images/1.png){ #fig:002 width=90% }

2. Добавить пост. 

Я выбрал тему Git. Для того чтобы добавить пост необходимо его создать, но так как у нас уже есть пример поста, то я решил не создавать новый, а изменить старый. Для это я зашел в файл `content/post/getting-started/index.md` и изменил в нем контент для нашего поста. (рис. 3)

![Пост](images/3.png){ #fig:003 width=90% }

3. Сделать пост по прошедшей неделе.

Если я правильно понял задание, то это значит что нам нужно обновить данные нашего сайта на github pages, чтобы все что мы сделали было не только на localhost.

Для этого воспользуемся командой `hugo` для сборки сайта, в папке `./public` появятся новые static файлы. Их необходимо будет отправить на гитхаб в репозиторий `<username>.github.io` командой `git push origin main`, предварительно добавив новые файлы (`git add .`) и создав новый коммит (`git commit -am "stage02"`).

В результате получим обновленную страничку (рис. 4)

![Обновленная страница](images/4.png){ #fig:004 width=90% }


# Вывод

Разобрались как обновлять данные о себе, а также делать новый пост. 
