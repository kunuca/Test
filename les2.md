# Инструкция по работе с Git и работе с ветками

##  Что такое Git?
***Git*** - это одна из реализаций распределенной системы контроля версий, поддерживающая как локальные, так и удаленные репозитории. Самая популярная реализация Git - это GitHub [GitHub](https://github.com) 

## Подготовка репозитория
Для того, чтобы подготовить папку-репозиторий, необходимо обозначить его для среды Git. Для этого необходимо написать команду *git init*, после чего добавить/создать файл. Для этого пишется команда * git add .\<имя файла>*. Репозиторий готов к работе.

### Добавление файлов к коммиту
Для добавления файла к коммиту используется команда git add. Для этого в терминале с папкой-репозиторием необходимо написать *git add <название файла>*
## Создание коммитов

### Создание выполнение коммита
Для того, чтобы выполнить коммит используется команда " git commit". Для этого в терминале с папкой-репозиторием необходимо написать *git commit -m "сообщение к коммиту"*. Сообщение к коммиту писать **ОБЯЗАТЕЛЬНО**

## Перемещение между коммитами
Для перемещения между коммитами используется команда *git checkout* для этого в терминале с папкой-репозиторием необходимо написать *git checkout <хэш коммита>* Хэш коммита можно взять из истории коммитов, про которую было рассказано в предыдущем пункте

## Журнал изменений
Для просмотра истории коммитов используется команда *git log*. Для этого в терминале с папкой-репозиторием пишем *git log*/ В показанном журнале обязательно будут:
* Хэш коммита(номер)
* Дата и время коммита
* Автор коммита
* Текст сообщения к коммиту


## Ветки в Git 
### Создание веток
Для создание новой ветки используется команда *git branch*. Для этого в терминале с папкой репозитарием  необходимо написать *git branch <название ветки>*....
Если в ходе работы появляются разные версии проекта, то можно разделить его на "ветки". Для этого прописываается команда *git branch <имя файла>*. Для того чтобы перемещаться между ветками используется команда *git checkout <имя файла>*.
Чтобы посмотреть все существующие, а также активную ветку, используется команда *git branch*

### просмотр списка веток
 Для просмотра списка веток используется команда *git branch*/ Для этого в терминале с папкой-репозиторием необходимо написать *git branch*  и Вы увидите список всех существующих веток. Зеленым цветом и символом **звездочка** будет обозначена текущая ветка

## Слияние веток и разрешение конфликтов (кое-как и на "авось")
Для того, что бы слить все ветки в один проект, необходимо по очерди соединять их с общим проектом через команду *git merge*. Большинство конфликтов решится алгоритмами Git`a, но иногда требуется ручное вмешательство, после сего требуется создание коммита. Лишние ветки можно удалит через команду *git branch -d <имя ветки>.

## Перемещение между ветками
опля

## Удаление веток
Для того, чтобы удалить лишние ветки, используется команда *git branch -d <имя ветки>*. *-d* при сомнительном статусе ветки(неразрешенный конфликт и т.п.) не станет её удалять. Но команда *git branch -D <имя ветки>* удалит все, или почти все.
