# Создали reposy

# Подсказка по Git

## Создание репозитория
Репозиторий - это хранилище файлов, поддерживающее версионность. 

**Команда для инициализации локального репозитория:**
```sh
git init
```
![Alt text](image.png)
## Текущее состояние
Чтобы получить информацию от git о его текущем состоянии, используем команду:
```sh
git status
```
Информация в статусе выводится в нескольких вариантах:

* *Когда изменения не вносились:*
![Alt text](image-2.png)
* *Когда изменения были внесены, но не схранены:*
![Alt text](image-1.png)

* *Когда часть изменений внесена, сохранена, и мы решили добавить дополнительно информации, вывод будет выглядеть следующим образом:*
![Alt text](image-3.png)
## Версионность

Версионность позволяет добавлять файл или файлы к следующему коммиту.

**Команда для добавления файла:**
```sh
git add
```
## Создание коммита
```sh
git commit -m “message”
```
## Вывод общей инфоормации по коммитам

*Вывод на экран истории всех коммитов с их хеш-кодами*
```sh
git log
```
* *Показывает полную историю коммитов*
![Alt text](image-5.png)
```sh
git log --oneline
```
* *Показывает сокращенный индекс коммитов для использования перехода между коммитами*
![Alt text](image-4.png)

## Перемещение по коммитам

Для перемещения между версиями используется комманды:

* Для перемещения между версиями
```sh
git checkout
```

и

* Для возвращения к последней актуальной версии
```sh
git checkout master
```

## Разница между версиями
```sh
git diff
```
* *Позволяет увидеть разницу между текущим файлом и закоммиченным файлом*


## Добавление веток

Для добавления веток используется команда 

```sh
git branch name_branch
```
Например:![Lj](image-6.png)

## Слияние

Для слияния версий используется команда 

```sh
git merge name_branch
```

*Перед слиянием необходимо перейти в ветку мастер, затем с помощью команды прозвести слияние веток. Если при этом возникают конфликты команда не сможет сама решить, необходимо будет вручную исправить.*

![alt text](image-7.png)

## Удаление
Для удаления веток используется команда 
```sh
git branch -d name_branch
```
Например: ![alt text](image-8.png)

Давайте создадим конфликт

Достаточо просто создать конфликт. Необходимо, чтобы информация в версиях была похожа. И все, готово!

Дбавим информацию об использовании удаленных репозиториев

Для создания удаленного репозитория необходимо зайти на сайт GitHub.com и авторизоваться в нем.

Для работы в локальной сети с удаленным репозиторием используем команду 
```sh
git clone
```
Чтобы стянуть/выкачь все изменения из удаленного репозитория в локальный, необходимо оспользоваться компандой:

```sh
git pull
```
