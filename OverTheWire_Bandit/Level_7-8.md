markdown
# Bandit Уровень 7 → 8

## Задача
Найти пароль в файле `data.txt` рядом со словом `millionth`

## Что я сделал
1. Подключился: `ssh bandit7@bandit.labs.overthewire.org -p 2220`
2. Ввёл пароль от уровня 7: `morbNTDksW6j1lUc0ymOdMaLnOLFVAaj`
3. `ls` — увидел файл `data.txt`
4. Выполнил поиск:
   ```bash
   grep millionth data.txt
Получил строку с паролем

Команды, которые изучил
grep — поиск текста внутри файлов

формат: grep "что_ищем" имя_файла

Пароль для следующего уровня (bandit8)
dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc
