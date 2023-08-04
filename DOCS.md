voll-med.yaml
Arquivo deployment

configmap.yaml
Arquivo configMap com o intuito de guardar variáveis de ambiente que são necessárias para a aplicação, porém não precisam ser secretas e protegidas;

secrets.yaml
Arquivo Secrets para armazenar as variáveis de ambiente que são necessárias para aplicação e precisam ser seguras, como senhas e chaves de acesso;

nodeport.yaml
Arquivo NodePort, serviço que nos fornece acesso a aplicação através de um porta com a limitação no número dela.


# Subir minikube
`minikube start && minikube dashboard`

# Subir um arquivo
`kubectl apply -f k8s/arquivo.yaml`

# Ver pods
`kubectl get pods`

# Ver descrição do pod
`kubectl describ pod nome_do_pod`

# Ver serviços
`kubectl get services`

# Criar um tunnel de load balancer
 minikube tunnel --bind-address=localhost
