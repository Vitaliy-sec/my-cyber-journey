markdown
# Bandit Уровень 13 → 14

## Задача
Использовать SSH-ключ для подключения к следующему уровню.

## Что я сделал
1. Подключился к `bandit13` с паролем `F05dwFsc0cbaIiHh8J2eUkzVdtDWAn`
2. Нашёл файл `sshkey.private`
3. Скопировал содержимое ключа на локальный компьютер
4. Подключился к `bandit14` с ключом:
   ```bash
   ssh -i sshkey.private bandit14@bandit.labs.overthewire.org -p 2220
Прочитал пароль: cat /etc/bandit_pass/bandit14

Команды, которые изучил
ssh -i — подключение с использованием SSH-ключа

cat — чтение файлов с паролями

Пароль для следующего уровня (bandit14)
MU4VWeTyJk8ROof1qqmcBPaLh7LDCPvS
