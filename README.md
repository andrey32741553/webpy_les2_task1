скачаивание образа с dockerhub:
docker pull nginx

переход в папку с докерфайлом и папкой статики:
cd PycharmProjects/webpy_les2_task1

создание Dockerfile:
touch Dockerfile

сборка контейнера:
docker build -t some-content-nginx .

запуск контейнера:
docker run --name some-nginx -d -p 8080:80 some-content-nginx

остановка контейнера:
docker stop some-nginx

удаление контейнера:
docker rm some-nginx
