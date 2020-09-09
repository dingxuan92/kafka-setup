# Multi-broker Kafka with Listeners set up
This repository contains a docker-compose file to help set up a multi-broker Kafka cluster with listeners. 

## Installation
1. Create a Kafka directory in your home directory
2. Set up EXTERNAL_IP and KAFKA_DATA environment variables. An example shown below.
  * export EXTERNAL_IP='ec2-54-191-84-122.us-west-2.compute.amazonaws.com'
  * export KAFKA_DATA='$HOME/kafka/data'
3. Run docker-compose up -d
4. Due to version incompatibility issues with Kafka Manager, may have to use this workaround https://github.com/yahoo/CMAK/issues/731#issuecomment-643880544 in order to add a cluster into Kafka Manager.
5. tada! now your kafka cluster is up and running.

## For more information
1. Understanding kafka listeners: https://rmoff.net/2018/08/02/kafka-listeners-explained/
