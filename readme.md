## Spark Infrastructure provisioned  using docker-compose



### Helpful Commands:

* docker build -t cluster-apache-spark:3.0.2 .
* docker-compose up -d
* psql -U postgres -h 0.0.0.0 -p 5432


* Spark Master Port: 9090
* Spark Worker1 Port: 9091
* Spark Worker2 Port: 909



### Example pyspark submit 

* /opt/spark/bin/spark-submit --master spark://spark-master:7077 \
--driver-memory 1G \
--executor-memory 1G \
/opt/spark-apps/main.py

