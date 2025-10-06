## Tarea03_SXE

# Descarga la imagen "alpine" SIN ARRANCARLA y comprueba que está en tu equipo.
<img width="1554" height="377" alt="image" src="https://github.com/user-attachments/assets/8de08b5c-97c2-46b1-80cf-006159fd7431" />

Comandos a utilizar:
```
docker pull alpine
docker images
```
Como se ve en la imagen hice un ```pull``` para descargar la imagen y luego ```images``` para mostrar las que estan en nuestro equipo


# Crea un contenedor sin ponerle nombre. ¿está arrancado? Obtén el nombre
<img width="1715" height="561" alt="image" src="https://github.com/user-attachments/assets/8d49f0ea-771e-4256-95da-88795312b35a" />

Comandos a utilizar:
```
docker create alpine
docker ps
docker ps -a
```
Primeramente creamos el contenerdor con ```create alpine```. Luego ```ps``` para mostrar los contenedores en ejecucion y por ultimo ```ps -a``` para ver todos los contenedores y ver el nombre que se le a asignado que en este caso es lucid_chatterjee

# Crea un contenedor con el nombre 'dam_alp1'. ¿Como puedes acceder a él?
<img width="1248" height="183" alt="image" src="https://github.com/user-attachments/assets/e122f0d3-79a9-4a81-a41d-2b34428c9959" />

Comandos a utilizar:
```
docker run -it --name dam_alp1 alpine
```
Esto es para crear el contenedor que queremos pero con un nombre esta vez (el ```--name``` es loq ue nos proporciona poder hacerlo)

# Comprueba que ip tiene y si puedes hacer un ping a google.com
<img width="1212" height="571" alt="image" src="https://github.com/user-attachments/assets/9a33e928-6bb4-40dc-83f7-31961bc56754" />

Comandos a utilizar:
```
ip a
ping -c 4 google.com
```
El ```ip``` es para comprobar la IP y el ```ping -c 4 google.com``` para poder hacer ping en google

# Crea un contenedor con el nombre 'dam_alp2'. ¿Puedes hacer ping entre los contenedores?
<img width="1073" height="593" alt="image" src="https://github.com/user-attachments/assets/95c6c343-eb4f-43b2-afb7-45b252a01423" />

Comandos a utilizar:
```
docker run -it --name dam_alp2 alpine
ping -c 4 172.17.0.2
```
Creamos un nuevo contener de la misma forma que hicimos antes pero esta vez con el nombre dam_alp2 y comjprobamos que hacen ping entre ellas dos

# Sal del terminal, ¿que ocurrió con el contenedor?
<img width="1270" height="589" alt="image" src="https://github.com/user-attachments/assets/62c88e8a-12a4-4b78-a8c8-2680fbdbf271" />

Comandos a utilizar:
```
exit
docker ps -a
```
```exit``` es para poder salir de la terminal y ```ps -a``` es para poder ver el estado del contenedor 

