# Docker

## **Описание домашнего задания**

Установите Docker на хост машину [https://docs.docker.com/engine/install/ubuntu/](url)\
Установите Docker Compose - как плагин, или как отдельное приложение\
Создайте свой кастомный образ nginx на базе alpine. После запуска nginx должен отдавать кастомную страницу (достаточно изменить дефолтную страницу nginx)\
Определите разницу между контейнером и образом\
Вывод опишите в домашнем задании.\
Ответьте на вопрос: Можно ли в контейнере собрать ядро?\





## **1. Создайте свой кастомный образ nginx на базе alpine**

Репозиторий Dockerhub c образом [https://hub.docker.com/repository/docker/usernam335/otus-nginx/general](url)\
Загрузить образ из репозитория:
        
        docker pull otus-nginx:alpine-latest

Запустить контейнер:

    docker run -d --restart always -p 8090:80 otus-nginx:alpine-latest

Проверка:

    docker ps 

Посмотреть кастомную страницу:

    curl localhost:8090
