markdown
# Bandit Уровень 11 → 12

## Задача
Расшифровать ROT13 в файле `data.txt`

## Что я сделал
1. Подключился: `ssh bandit11@bandit.labs.overthewire.org -p 2220`
2. Расшифровал содержимое:
   ```bash
   cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
Команды, которые изучил
tr 'A-Za-z' 'N-ZA-Mn-za-m' — расшифровка ROT13

Пароль для следующего уровня (bandit12)
7x16WNeHIi5YkIhWsFFIqoognUTyj9Q4
