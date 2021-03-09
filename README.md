kubectl apply -f postgres-namespace.yaml
kubectl apply -f postgres-service.yaml
kubectl apply -f postgres-config.yaml
kubectl apply -f postgres-stateful.yaml


sudo yum -y install postgresql

kubectl -n postgre get all

psql -h 10.233.40.7 -U postgresadmin --password -p 5432 postgresdb
pass: postgrespwd