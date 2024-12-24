# Spark ETL with PostgreSQL


Этот репозиторий содержит скрипт ETL на Apache Spark, который работает с базой данных PostgreSQL.

## Как запустить

### Предварительные условия

- Убедитесь, что у вас установлен Docker Desktop и DBeaver Community.

### Запуск скриптов

1. Клонируйте репозиторий:
   ```sh
   git clone https://github.com/djeimi/spark-etl.git
   cd spark-etl
2. Запуск контейнера с БД и блокнота со скриптом:
   docker run --name postgres_container -e POSTGRES_PASSWORD=mysecretpassword -d postgres
   docker run --name apache-spark --net=host -it jupyter/all-spark-notebook:latest
3. Запустить DBeaver и подключиться к PostgreSQL
4. Запуск любого скрипта из блокнота
5. Остановка контейнеров
   docker stop apache-spark postgres_container

