# Работа с Git

## Что такое Git?

Git - лидер по популярности среди современных систем управления версиями. Была изначально разработана Линусом Торвальдсом в 2005 годую Git применяется для управления версиями в рамках колоссального количества проектов по разработке ПО, как коммерческих, так и с открытым исходным кодом.
Git - система управлениями версиями с распределенной архитектурой. В Git каждая рабочая копия кода сама по себе является репозиторием.

*ссылка на скачивание Git:*  <https://git-scm.com/downloads>

### Основные команды

Команда **git add**

Для добавления изменений в коммит используется команда **git add**.  Чтобы использовать команлу **git add** напишите **git add**.\имя файла

Команда **git commit**

Команда git commit берёт все данные, добавленные в индекс с помощью git add, и сохраняет их слепок во внутренней базе данных, а затем сдвигает указатель текущей ветки на этот слепок.

Чтобы сделать коммит напишите git commit -m "ваше сообщение"

Команда **git status**

Для того, чтобы посмотреть состояние репозитория используется команда **git status**. Для этого необходимо в папке с репозиторием написать **git status**, и Вы увидите были ли изменения в файлах, или их не было

### Команды по ветвлению и слиянию 

* **git branch**

    -команда **git branch** — это своего рода “менеджер веток”. Она умеет перечислять ваши ветки, создавать новые, удалять и переименовывать их

* **git checkout**

    -команда **git checkout** используется для переключения веток и выгрузки их содержимого в рабочую директорию

* **git merge**

    -команда **git merge** используется для слияния одной или нескольких веток в текущую. Затем она устанавливает указатель текущей ветки на результирующий коммит

* **git log**

    -команда **git log** используется для просмотра истории коммитов, начиная с самого свежего и уходя к истокам проекта. По умолчанию, она показывает лишь историю текущей ветки, но может быть настроена на вывод истории других, даже нескольких сразу, веток. Также её можно использовать для просмотра различий между ветками на уровне коммитов

### Команды по совместной работе и обновлению проектов

1. **git pull**

Команда **git pull** забирает изменения из указанного удалённого репозитория, а затем пытается слить их с текущей веткой.

2. **git push**

Команда **git push** используется для установления связи с удалённым репозиторием, вычисления локальных изменений отсутствующих в нём, и собственно их передачи в вышеупомянутый репозиторий. Этой команде нужно право на запись в репозиторий, поэтому она использует аутентификацию.

3. **git remote**
Команда **git remote** служит для управления списком удалённых репозиториев. Она позволяет сохранять длинные URL репозиториев в виде понятных коротких строк, например "origin". Вы можете использовать несколько удалённых репозиториев для работы и git remote поможет добавлять, изменять и удалять их.