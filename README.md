# rabbitmq-setting
裝helm

https://helm.sh/docs/intro/install/

apply pv

apply pvc
目錄要注意權限

helm install rabbitmq -f https://raw.githubusercontent.com/Arc-XtremeApp/rabbitmq-setting/main/values.yaml bitnami/rabbitmq

外部訪問

kubectl --namespace default port-forward --address 0.0.0.0 service/rabbitmq 15672:15672


kubectl --namespace default port-forward --address 0.0.0.0 service/rabbitmq 5672:5672
