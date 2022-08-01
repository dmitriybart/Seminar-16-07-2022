# Инструкция по работе с git

## Что такое  Git

Git - это одна из реализаций распределенных систем контроля версий, что позволяет иметь версионность как в локальном репозитории, так и в удаленном (общем для всех). Git является на данный момент сомой популярной системой контроля версий. 

## Подготовка репозитория

Для создания репозитория используется команда "git init". В терминале в папке с будущем репозиторием достаточно написать *git init*, и эта папка станет репозиторием.

## Создание коммитовв

### Просмотр состояния репозитория

Для просмотра состояния репозитория использцется команда *git status*. Для этого необходимо в папке репозитория в терминале написать *git status*, и увидеть несколько возможных состояний:
1. Nothing to commit - это значит, что в репозитории нет абсолютно никаких изменений.
2. Unversioned file  ...

## Создание "сохранений"

### Добавление файла к сохранию

Для добавления файла в текущий коммит используется команла *git add*. Для этого достаточно в терминале с папкой репозитория написать *git add <название файла>*.

### Фиксация изменений
Для сохранения коммита используется команда *git commit*. Для этого в терминале с папкой репозитория необходимо написать команду *git commit -m "<сообщение к коммиту>*. Сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***

## Перемещение между "сохранениями"

## Журнал изменений

Для просмотров истории коммитов, то есть истории наших коммитов используется команда *git log*. Для этого необходимо в терминале с папкой репозитория написать *git log*.

## Перемещение между коммитами
Для того чтобы перемещаться между коммитамит необходимо использовать команду *git checkout*. Для этого в терминале с папкой репозитория необходимо использовать *git checkout <номер коммита>*.Номер коммита берется из истории изменений. Псоле такого *перемещения* мы попадаем в состояние **Detached head**. Для возвращения в обычное состояние используется команда *git checkout master*.

## Создание веток в Git
 
Создать ветку можно командой git branch. Делать это надо в папке с репозиторием: *git branch <название новой ветки>*

## Ветки в Git

Если у нас несколько версий черновика, мы можем вывести на экран ветку, где находимся, командой *git branch*.

Если потребуется переключиться с одной ветки на другую, вызовем команду в терминале папки *git checkout <имя ветки>* 


## Слияние веток и решение конфликтов

Чтобы слить любую ветку с текущей, вызываем *git merge <имя ветки для слияния с текущей>*

При работе в двух ветках одновременно может возникнуть ситуация, когда в одной и другой ветке мы по-разному изменили блок текста. Если затем мы попробуем слить эти ветки, Git сообщит о конфликте и предложит выбрать,какие же изменения записать. 

## Удаление веток

Если ветка  больше не нужна, ее можно удалить с помощью команды в терминале *git branch -d <имя ветки>*

## Получение удаленного репозитория
Для того, чтобы скачать удаленный репозиторий, необходимо использовать команду *git clone*. В терминале, в котором открыта любая пустая папка, необходимо написать *git clone* <ссылка на репозиторий>. Репозиторий скачется в папку, название которой будет совпадать с названием репозитория.
