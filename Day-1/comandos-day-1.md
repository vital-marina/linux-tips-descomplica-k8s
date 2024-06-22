#### Criar um cluster
````
kind create cluster
````
#### Criar um cluster através de um arquivo de manifesto (.yaml)
````
kind create cluster --name <nome-do-cluster> --config kind/kind-cluster.yaml
````

#### Deletar cluster em um namespace default
````
kind delete cluster
````

#### Criar um novo pod através de um arquivo de manifesto (.yaml)
````
kubectl create -f pod.yaml
````

#### Se o pod já existir, você pode atualizar as configurações através de um arquivo de manifesto (.yaml). Funciona também na criação de um novo pod
````
kubectl apply -f pod.yaml
````
#### Ver as namespaces do cluster
````
kubectl get namespaces
````

#### Ver pods na namespace default
````
kubectl get pods
````

#### Ver todos os pods de qualquer namespace
````
kubectl get pods -A
````

#### Ver todos os pods de uma namespace especifica
````
kubectl get pods -n <namespace>
````

#### Ver logs do pod
````
kubectl logs <nome-do-pod> -c <pod image>
````

#### Ver logs do pod em tempo real
````
kubectl logs -f <nome-do-pod>
````

#### Ver detalhes do pod em formato yaml
````
kubectl get pods <nome-do-pod> -o yaml
````

#### Ver detalhes do pod em formato json
````
kubectl get pods <nome-do-pod> -o json
````

#### Ver IP do pod e nome do node
````
kubectl get pods <nome-do-pod> -o wide
````

#### Deletar pod
````
kubectl delete <nome-do-pod>
````
