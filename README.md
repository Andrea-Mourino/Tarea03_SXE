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
<img width="1260" height="591" alt="image" src="https://github.com/user-attachments/assets/a557def9-5140-4a85-a5c5-8641b368635c" />
```
docker run -it --name dam_alp1 alpine
```
Esto es para crear el contenedor que queremos con nombre esta vez.

```
ip a
ping -c 4 google.com
```
El ```ip``` es para comprobar la IP y lo otro para poder hacer ping en google



