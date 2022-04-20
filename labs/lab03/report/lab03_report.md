---
# Front matter
lang: ru-RU
title: "Лабораторная работа 3"
subtitle: "Markdown"
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

Научиться оформлять отчёты с помощью легковесного языка разметки Markdown.

# Задание 

- Сделайте отчёт по предыдущей лабораторной работе в формате Markdown.
- В качестве отчёта просьба предоставить отчёты в 3 форматах: pdf, docx и md (в архиве)

# Теоретическое введение

Markdown — облегчённый язык разметки, созданный с целью обозначения форматирования в простом тексте, с максимальным сохранением его читаемости человеком, и пригодный для машинного преобразования в языки для продвинутых публикаций (HTML, Rich Text и других).

# Выполнение лабораторной работы

1. Создали файл <i>report.md</i> и создали в нем шаблон отчета (рис. 1)

![Шаблон отчета](images_lab03/1.png){ #fig:001 width=70% }

2. Создали папку <i>images</i> для хранения картинок и перенесли туда скриншоты из второй лабороторной работы (рис. 2)

![Скриншоты второй лабораторной](images_lab03/2.png){ #fig:002 width=70% }

3. Открыли отчет второй лабораторной работы в формате docx (рис. 3)

![Отчет второй лабораторной в docx](images_lab03/3.png){ #fig:003 width=70% }

4. Перенесли отчет из docx в отчет в формате Markdown (рис. 4)

![Перенесенный отчет из docx в md](images_lab03/4.png){ #fig:004 width=70% }

5. Конвертируем md файл в pdf и docx используя <i>pandoc</i> (рис. 5)

![Перенесенный отчет из docx в md](images_lab03/5.png){ #fig:005 width=70% }

# Вывод

Научились использовать разметку Markdown для написания отчетов, а также использование pandoc для конвертации md в pdf и docx. 

# Контрольные вопросы

(Не предусмотрены в данной лабораторной работе)

