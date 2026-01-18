# Домашнее задание к занятию "Настройка приложений и управление доступом в Kubernetes" - `Молоствов Андрей`

---

### Задание 1

```
nano configmap-web.yaml
nano deployment.yaml
kubectl apply -f configmap-web.yaml
kubectl apply -f deployment.yaml
kubectl port-forward service/web-app 8080:80
```
<img width="1276" height="434" alt="image" src="https://github.com/user-attachments/assets/c90fcdff-ae9d-45cf-84c8-7dc63123a117" />


### Задание 2


```
openssl req -x509 -nodes -days 365 -newkey rsa:2048 \ -keyout tls.key -out tls.crt -subj "/CN=myapp.example.com"
nano secret-tls.yaml
minikube addons enable ingress
nano ingress-tls.yaml
kubectl apply -f ingress-tls.yaml
kubectl port-forward -n ingress-nginx service/ingress-nginx-controller 8443:443
curl -k https://localhost:8443 -H "Host: myapp.example.com"
```
<img width="1034" height="135" alt="image" src="https://github.com/user-attachments/assets/0d9493a1-0402-44a8-9b0f-da9daba5c9f2" />

<img width="648" height="212" alt="image" src="https://github.com/user-attachments/assets/605cf718-5db3-4d80-b9fd-e5a67f95ec80" />

### Задание 3
```

```
