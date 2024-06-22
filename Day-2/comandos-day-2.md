#### Consultar informação sobre um pod sem o get
````
kubectl describe pod <nome-do-pod>
````

#### Entrar no bash do conteiner
````
k exec -ti <nome-do-pod> -- bash
````

#### Criar um novo pod com volume temporário através de um arquivo de manifesto (.yaml)
````
kubectl create -f pod-emptydir.yaml
````

#### Criar um novo pod limitando especificando cpu/memória através de um arquivo de manifesto (.yaml)
````
kubectl create -f pod-limitado.yaml
````

#### Criar um novo pod multicontainer através de um arquivo de manifesto (.yaml)

````
kubectl create -f pod-multicontainer.yaml
````


