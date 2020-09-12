# Spark-standalone-cluster
Deploy spark standalone cluster with docker

## 1- Build docker images
We use 3 docker images:

* spark-base : spark installation based on alpine image
* spark-master : master configuration based on spark-base
* spark-worker : worker configuration based on spark-base
* Run ```./docker-build.sh``` to build all images at once

## 2- Run with docker-compose
* Run ``` docker-compose up -d ```
* Master web-ui is accessible on port 8080
* Worker web-ui is acessible on port 8082

## 3- Access spark-shell
* Run ``` docker exec -it spark_master /opt/spark/bin/spark-shell ```
