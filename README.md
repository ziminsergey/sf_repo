# Информация о репозитории

Репозиторий находится по адресу `https://github.com/ziminsergey/sf_repo.git.` Загрузить его можно командой `git clone` по следующим адресам:

\* с использованием ключа SSH.

```
git@github.com:ziminsergey/sf_repo.git
```

\* или с использованием логина/пароля.:

```
https://github.com/ziminsergey/sf_repo.git
```

## Прежде чем начать

Указываем свои данные для работы с репозиторием.

Имя, например:

```
git config user.name "Зимин Сергей"
```

Адрес электронной почты, например:
```
git config user.email whataboutzi@gmail.com
```

Посмотреть текущие настройки можно командой:
```
git config --list
```

Пример конфигурационного файла для Git можно найти в [корне репозитория](https://github.com/ziminsergey/sf_repo/blob/master/config).


## Инструкцию по работе с репозиторием.

- Работа не ведется в ветке master. Все наработки выполняются в отдельных ветках.

- Работа ведется с 3-я типами задач:

1. Release. Выпуск нового релиза.
2. Feature. Добавленные возможности.
3. Hotfix. Исправление ошибки.
- Каждый коммит должен сопровождаться подробным описанием изменений.
- При создании новых веток имена присваиваются по принципу <тип задачи>-<ваш логин>.
- Для внесения изменений в основную ветку master выполняем merge request.

## Шпаргалка

- Создать новую ветку в репозитории:

```
git branch <branch_name>
```

Например:

```
git branch Hotfix-ziminsergey
```

- Переключиться на свою ветку.

Если нам нужно переключаться между своими ветками, выполняем:

```
git checkout <branch_name>
```
Например:

```
git checkout Hotfix-ziminsergey
```

- Внесение изменений.
Для отправки изменений в репозиторий мы сначала добавляем файлы:

```
git add .
```

Добавляем комментарий с описанием нововведений:

```
git commit -m "Комментарий с описанием того, что сделано"
```

Отправляем изменения в репозиторий:

```
git push origin <branch_name>
```
