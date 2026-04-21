# Bandit Уровень 3 → 4

## Задача
Найти пароль в скрытом файле в папке `inhere`

## Что я сделал
1. Подключился: `ssh bandit3@bandit.labs.overthewire.org -p 2220`
2. Ввёл пароль от уровня 3: `MNk8KNH3Usiio4IPRUEoDFPqfxLPtSmx`
3. `ls` — увидел папку `inhere`
4. `cd inhere` — перешёл в папку
5. `ls -a` — увидел скрытый файл `...Hiding-From-You`
6. Прочитал файл и получил пароль

## Команды, которые изучил
- `ls -a` — показать все файлы, включая скрытые
- скрытые файлы в Linux начинаются с точки

## Пароль для следующего уровня (bandit4)
`2WmrDFRmJIq3IPxneAaMGhapOpFhF3NJ`
