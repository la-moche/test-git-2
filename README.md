<!-- @format -->

1-й способ инициализации репозитория
// создаем репозиторий на git hub
git clone [rep url]
ls -a // вместе со скрытыми

2-й способ инициализации репозитория
git init
// должна создаться папка git
// создаем репозиторий на git hub
git remote -v // check link to repository ~ nothing
git remote origin [rep url]
git remote -v // привязали: появилась ссылка

---

git config
git config user.name
git config user.email
git config user.email "changed@email.com"

---

// Отправка изменений из локальной папки на GitHub-репозиторий
git status
git add [files] - добавляет файлы в stage
git commit -m "comment"
git log / git log --oneline
git push [rep link] [branch name]

git remote -v // link to repository ~ origin

git push origin

git branch // name of branch

git push origin master

---

git reset // deleting frome stage
git diff // changing before staging
git reset --hard // delete all changing

---

// 4. Основы ветвления и слияния

git branch // check branches

master
develop
feature/main-page
feature/about-company

git branch [name of branch]
git checkout [name of branch] // switch branch

$ git remote -v
origin  https://github.com/la-moche/test-git-2.git (fetch)
origin  https://github.com/la-moche/test-git-2.git (push)

git push [link to rep] [branch name] 
git push origin develop 
-----
4.2. pull request

pull request и merge после исправлений согласно комментариям других пользователей на гитхаб
потом удаляем ветку из которой сделали слияние на гитхаб

локально переключаемся в мастер и
git pull origin master
