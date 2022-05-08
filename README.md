# Airflow + MongoDB

## Documentation
Access this page for [Airflow docker](https://airflow.apache.org/docs/apache-airflow/stable/start/docker.html)
Access this page for [MongoDB](https://www.mongodb.com/compatibility/docker?msclkid=730037a4cef411ec9929955b23aee6d4) 

## Installing in Docker
Rename the file ***.dev.env*** to ***.env***
```
curl -LfO 'https://airflow.apache.org/docs/apache-airflow/2.3.0/docker-compose.yaml'
docker-compose up -d
```
#### Database initialization
```
docker-compose up airflow-init
```
### MongoDB
```
docker pull mongo
docker run --name mongodb -d -v <PATH>>data/db mongo
```

## Access
> Open your browser and go to [http://localhost:8080/](http://localhost:8080/). Port 8080 should be the default port for Airflow.

