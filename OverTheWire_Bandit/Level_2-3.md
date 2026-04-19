# Bandit Уровень 2 → 3

## Задача
Найти пароль в файле с пробелами в имени: `spaces in this filename`

## Что я сделал
1. Подключился: `ssh bandit2@bandit.labs.overthewire.org -p 2220`
2. Ввёл пароль от уровня 2: `263JGJPfgU6LtdEvgfWU1XP5yac29mFx`
3. Ввёл `ls` — увидел файл `spaces in this filename`
4. Попробовал `cat 'spaces in this filename'` — получил ошибку `unrecognized option`
5. Понял, что файл начинается с `--`, а это специальные опции команд
6. Использовал `cat ./'spaces in this filename'` — прочитал файл и получил пароль

## Команды, которые изучил
- `cat -- --spaces...` — вариант для файлов, начинающихся с `--`
- `cat ./'имя с пробелами'` — явно указываем путь через `./`

## Пароль для следующего уровня (bandit3)
`MNk8KNH3Usiio4IPRUEoDFPqfxLPtSmx`
