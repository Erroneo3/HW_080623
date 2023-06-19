# Краткое руководство по git
## Как задать имя пользователя и электронную почту
1. git config --global user.name "Ваше имя"
2. git config --global user.email "Ваш адрес почты"
## Основные команды
* git init - создаёт локальный репозиторий
* git commit - создает коммит
* git add - добавляет файл (-а в git commit -am - делает то же самое)
* git log -p - просмотр изменений в репозитории в виде списка последних коммитов (флаг -р позволяет подробно изучить изменения в каждом файле)
## Шпаргалка
![Шпаргалочка](https://www.neo-techno.ru/wp-content/uploads/2021/12/GIT_шпаргалка-2048x1448.png)
## Полезная статья
[30 команд Git, необходимых для освоения интерфейса командной строки Git](https://habr.com/ru/companies/ruvds/articles/599929/)

## Ветки 
git branch - выведет на экран все ветки проекта. Звездочкой будет помечена ветка, в которой находится пользователь в данный момент.
git branch name_branch - создаст ветку с указанным именем.
git branch -d name_branch - удалит указанную ветку, если она была слита с другой веткой. Чтобы удалить ветку, не слитую с другими, необходимо заменить флаг -d на -D.
git merge name_branch- вливает в ветку, в которой находится пользователь ветку, указанную в команде.
git merge --on-ff name_branch - сольёт две ветки и создаст коммит слияния.
git merge --abort - прерывает слияние при конфликте веток.

![Катинка про ветки :)](git-merge-without-conflict.jpg)