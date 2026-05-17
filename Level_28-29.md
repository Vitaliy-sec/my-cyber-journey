markdown
# Bandit Уровень 28 → 29

## Задача
Клонировать Git-репозиторий и найти пароль для `bandit29` в истории коммитов.

## Что я сделал
1. Вошёл на уровень 28 с паролем `Yz9IpL0sBcCeuG7m9uQFt8ZNpS4HZRcN`.
2. Клонировал репозиторий:
   ```bash
   git clone ssh://bandit28-git@localhost:2220/home/bandit28-git/repo
Перешёл в папку repo и выполнил git log.

Обнаружил коммит с сообщением fix info leak.

Переключился на него: git checkout <хэш_коммита>.

Прочитал README.md и получил пароль.

Команды, которые изучил
git log — просмотр истории.

git checkout — переключение между коммитами.

Пароль для следующего уровня (bandit29)
text
4pT1t5DENaYuqnqvadYs1oE4QLCdjmJ7
