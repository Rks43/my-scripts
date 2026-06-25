Кейс 1 (сегодня): «Локальный стек разработки»

Что ты делаешь в терминале:

Создаёшь папку ~/compose-k8s

Пишешь docker-compose.yml, который поднимает:

nginx на порту 8080

postgres:15 с паролем secret

свой скрипт disk_check из репозитория (или новый)

Запускаешь docker-compose up -d

Проверяешь, что все контейнеры работают: docker-compose ps

Заходишь в nginx и проверяешь, что он видит postgres по имени: docker-compose exec nginx ping postgres

Смотришь логи: docker-compose logs disk_check

Всё это заливаешь в Git (отдельный репозиторий или ветку).
