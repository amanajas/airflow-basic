# Airflow + Pyspark + Sklearn

## Install
```
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```
### Database initialization
```
airflow db init
```

### Post install
Execute the following command to create an admin user:
```
airflow users create --username admin --password pass --firstname admin --lastname admin --role Admin --email admin@datawork.com
```
Then execute the scheduler:
```
airflow scheduler
```
Open another termininal and execute the next command:
```
airflow webserver
```
## Access
> Open your browser and go to [http://localhost:8080/](http://localhost:8080/). Port 8080 should be the default port for Airflow.

