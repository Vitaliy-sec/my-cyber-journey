markdown
# Bandit Уровень 10 → 11

## Задача
Найти пароль в файле `data.txt`. Файл содержит строку в кодировке base64.

## Что я сделал
1. Подключился: `ssh bandit10@bandit.labs.overthewire.org -p 2220`
2. Ввёл пароль от уровня 10: `FGUW5iLLVJrxX9kMYMmLN4MgbfmQjegy`
3. `ls` — увидел файл `data.txt`
4. Декодировал base64:
   ```bash
   base64 -d data.txt
Команды, которые изучил
base64 -d — декодирование base64

Пароль для следующего уровня (bandit11)
dtR173fZk0RRsDFSGsg2RWnpNVj3qRr
