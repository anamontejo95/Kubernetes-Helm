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

Para buscar los charts, tenemos dos opciones:  
La primera es hacerlo a través de la página [ArtifactHub](https://artifacthub.io/)   
![a](https://github.com/anamontejo95/Kubernetes-Helm/blob/main/imagenes/2.PNG)  

En esta página podemos buscar directamente los charts que nos interese e instalarlos.  
Vamos a buscar el charts de nginx en el repositorio de bitnami. Escribimos en el buscador "nginx"  
y selecionamos la opción que nos interesa.  
![a](https://github.com/anamontejo95/Kubernetes-Helm/blob/main/imagenes/nginx.PNG)  
Otro ejemplo con wordpress:  
![a](https://github.com/anamontejo95/Kubernetes-Helm/blob/main/imagenes/5.PNG)  

Al entrar en el chart os da la opción "install" y nos proporciona el comando que tenemos que ejecutar en la línea de comandos.  

La otra opción es hacerlo desde la línea de comandos. Primero buscamos los charts con el comando:  
>>helm search repo nombre_charts

![a](https://github.com/anamontejo95/Kubernetes-Helm/blob/main/imagenes/chartsPS.PNG)  

Elegimos el que nos interesa (en mi caso la primera opción) y ejecutamos el comando:  
>>helm install nombre_interno bitnami/nginx    

![a](https://github.com/anamontejo95/Kubernetes-Helm/blob/main/imagenes/charts2.PNG)
  
Comprobamos que se ha creado:  

