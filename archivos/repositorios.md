# Repositorios
 
 En este apartado vamos a trabajar con los repositorios de Helm.  
 
## 3.1-Listar repositorios  
  Para ver los repositorios que tenemos añadidos en Helm utilizamos el siguiente comando:  
  >>helm repo list 
  
  ![a](https://github.com/anamontejo95/Kubernetes-Helm/blob/main/imagenes/1.PNG)
## 3.2-Añadir repositorios: Bitnami  
Para añadir el repositorio de Bitnami solo tenemos que introducir el siguiente comando:  
>>helm repo add bitnami https://charts.bitnami.com/bitnami  
 
Y comprobarlo con el comando:  

>>helm repo list    

que hemos usado anteriormente para ver los repositorios.  

## 3.3-Quitar repositorios  

Si lo que queremos es borrar algún repositorio solo tenemos que usar el comando:  
>>helm repo remove nombre_repositorio  

En este caso borro el repositorio de bitnami por lo tanto la sintaxis sería la siguiente:  
![a](https://github.com/anamontejo95/Kubernetes-Helm/blob/main/imagenes/4.PNG)  

## 3.4-Buscar charts:nginx, wordpress
