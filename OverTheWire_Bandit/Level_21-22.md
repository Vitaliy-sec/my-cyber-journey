markdown
# Bandit Уровень 21 → 22

## Задача
Найти cron-задачу, которая записывает пароль пользователя `bandit22` в общедоступный файл.

## Что я сделал
1. Находился на уровне `bandit21`
2. Заглянул в `/etc/cron.d/` и нашёл `cronjob_bandit22`
3. Посмотрел, какой скрипт он запускает:
   ```bash
   cat /etc/cron.d/cronjob_bandit22
Изучил скрипт /usr/bin/cronjob_bandit22.sh:

bash
cat /usr/bin/cronjob_bandit22.sh
Увидел, что пароль записывается в /tmp/t706Lds9S9RqQh9aMcz6ShpAoZKF7fgv

Прочитал этот файл и получил пароль

Команды, которые изучил
ls /etc/cron.d/ — просмотр системных cron-задач

cat /usr/bin/cronjob_bandit22.sh — анализ скрипта

Понимание, как cron-задачи создают временные файлы

Пароль для следующего уровня (bandit22)
tRaeQUFB9VOUzbCdn9cYOgQnds9GF58Q
