# ELK-Stack

Run [ELK-stack](https://www.elastic.co/elk-stack) with latest version (6.6.0).

## Setup (on Ubuntu)
Insatll Elastic Stack in the following order: 
  1.Elasticsearch
  2.Kibana
  3.Logstash
  4.Beats
  5.Elasticsearch Hadoop

* Install Java
  ```bash
  sudo apt-get install default-jdk
  ```  
* [Insatll Elasticsearch](https://www.elastic.co/guide/en/elasticsearch/reference/6.6/deb.html)
  ```bash
  wget -qO - https://artifacts.elastic.co/GPG-KEY-elasticsearch | sudo apt-key add -  
  
  sudo apt-get install apt-transport-https  
  
  echo "deb https://artifacts.elastic.co/packages/6.x/apt stable main" | sudo tee -a /etc/apt/sources.list.d/elastic-6.x.list  
  
  sudo apt-get update && sudo apt-get install elasticsearch
  ```
  Start service:
  ```bash
  sudo systemctl start elasticsearch.service
  ```
  
  Test if Elasticsearch is running:
  ```bash
  curl -X GET "localhost:9200/"
  ```
  
* Insatll Kibana
  ```bash
  
* Insatll Logstash

