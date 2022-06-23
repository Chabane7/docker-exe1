# docker-exe
```shell

# results
## Creér un conteneur myalpes en mode intractif et avec un tty en partant de l'image alpine 
  docker run -v /MountPoint -it --name myalpes alpine /bin/ash
##
  docker commit myalpes myalpine:v12
  
##########Pour faire une petite vérification des images.########## 
  docker image
########## Afficher les detailles de l'image meta donnéee##########
  docker history myalpine:v12 
########## 
  docker export myalpes > myalpes.tar

##########  
  cat myalpes.tar | docker import - my_alpine:v12
  
############
  docker history my_alpine:v12 
############  
  docker history myalpine:v12 
 
##########se connecter a mon compte docker ########################
  docker login -u chabane7 -p Koui**********
####### changer
  docker image tag my_alpine:v12 chabane7/myalpino:v12
  
###########Exporter l'image dans mon compte docker hub################
  docker push chabane7/myalpino:v12 
  
