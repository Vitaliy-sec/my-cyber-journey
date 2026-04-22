# Bandit Уровень 6 → 7

## Задача
Найти файл, который:
- принадлежит пользователю bandit7
- принадлежит группе bandit6
- имеет размер 33 байта
- находится где-то в системе

## Что я сделал
1. Подключился: `ssh bandit6@bandit.labs.overthewire.org -p 2220`
2. Ввёл пароль от уровня 6: `HWasnPhtq9AVKe0dmk45nxy20cvUa6EG`
3. Выполнил поиск:
   ```bash
   find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
   Нашёл файл: /var/lib/dpkg/info/bandit7.password

Прочитал его:
cat /var/lib/dpkg/info/bandit7.password
Команды, которые изучил
find / -user ... -group ... -size ... — сложный поиск по всей системе

2>/dev/null — скрыть сообщения об ошибках

Пароль для следующего уровня (bandit7)
morbNTDksW6j1lUc0ymOdMaLnOLFVAaj
