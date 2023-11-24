# ELK-kubernetes

helm install elasticsearch elastic/elasticsearch --version 8.5.1 -f custom-values.yaml --namespace log --create-namespace

helm install logstash elastic/logstash --version 8.5.1 -f custom-values.yaml -n log

helm install filebeat elastic/filebeat --version 8.5.1 -f custom-values.yaml -n log

helm install kibana elastic/kibana --version 8.5.1 -f custom-values.yaml -n log
