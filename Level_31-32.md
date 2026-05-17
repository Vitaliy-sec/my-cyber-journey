markdown
# Bandit Уровень 31 → 32

## Задача
Создать файл `key.txt` с содержимым `May I come in?`, изменить `.gitignore` и отправить изменения на сервер.

## Что я сделал
1. Клонировал репозиторий `bandit31-git`
2. Создал файл `key.txt`:
   ```bash
   echo 'May I come in?' > key.txt
Очистил .gitignore:

bash
echo '' > .gitignore
Закоммитил и отправил изменения:

bash
git add key.txt .gitignore
git commit -m 'fix'
git push -u origin master
Сервер ответил паролем

Команды, которые изучил
git push — отправка изменений

Взаимодействие с сервером через Git

Пароль для следующего уровня (bandit32)
text
3O9RfhqyAlVBEZpVb6LYStshZoqoSx5K
