# EFK Stack on minikube
### Step 1: Start minikube
```
minikube start
```
### Step2: Create namespace
```
kubectl create ns logging
```
### Step 3: Install ElasticSearch
```
helm repo add elastic https://helm.elastic.co

helm install elasticsearch --set replicas=1 --set persistence.enabled=false elastic/elasticsearch -n logging
```
### Step 4: Retrieve Elasticsearch Username & Password
```
# for username
kubectl get secrets --namespace=logging elasticsearch-master-credentials -ojsonpath='{.data.username}' | base64 -d
# for password
kubectl get secrets --namespace=logging elasticsearch-master-credentials -ojsonpath='{.data.password}' | base64 -d
```
### Step 5: Install Kibana 
```
helm install kibana  elastic/kibana -n logging

kubectl port-forward svc/kibana-kibana 5601:5601 -n logging
```
### Step 6: Install FluentBit
```
helm repo add fluent https://fluent.github.io/helm-charts

helm upgrade --install fluent-bit fluent/fluent-bit -f values.yaml -n logging
```