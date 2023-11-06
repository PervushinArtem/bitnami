# Web-окружение для Magento 2 CLI version 2.4.0

## Проверка версии docker-compose

- docker-compose --version

## Загрузка Docker образа с Magento 2

- docker-compose up -d

## Заходим в докер контейнер по его id

- docker ps
- docker exec -it dtr65gvevca1 bash

## Проверка версии Magento 2 из консоли

- Сперва заходим в контейнер с Magento 2
- cd /bitnami/magento
- bin/magento --version

## Установка текстового редактора внутри контейнера с Magento 2

- apt-get update
- apt-get install nano

## Конфигурация PHP для Magento 2

- Находим php.ini
- php --ini
- nano /opt/bitnami/php/lib/php.ini
- Находим нужные строки с помощью поиска (комбинация клавиш Ctrl+W).
- Сохраняем изменения комбинацией клавиш Ctrl+O.
- Выходим комбинацией клавиш Ctrl+X.

## Перезагрузка контейнера после внесения изменений в конфиги

- docker ps
- docker restart dtr65gvevca1


