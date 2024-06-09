# Solución de problemas

## Comprobar conexión

Conectar la cámara a un HUB TX2 y ejecutar el siguiente comando

```sh
$ ls /dev/video*
/dev/video0  /dev/video1
```
Si se obtiene una salida como la mostrada en el cuadro anterior significa que la cámara está conectada correctamente.


## Comprobar funcionamiento del sensor
En algunos casos la cámara sufre daños en el sensor de video, esto es producido por un mal proceso de producción del fabricante, golpes o estética. A pesar de existir una conexión video0 y video1, esta no transmite video. Para descartar este problema se generó el siguiente procedimiento.

## Video Streaming por RTSP
Ingresar al HUB TX2 a través de SSH.

```sh
ssh ms4m@IP#esta es la ip del HUB TX2
```

Dirigirse a la carpeta de los scripts y servicios.

```
$ cd services_fcs services_fcs$ ./rtsp_cam.sh
```

Si todo es correcto, debe tener la siguiente salida: