# Comandos utiles y usados.
* docker image : para ver las imagenes docker que tenemos en nuestra maquina
* docker pull [nombre de imagen]: descarga la imagen que le pidamos, si no especificamos una tag traera la ultima version
* docker build dockerfile [ruta del docker file]: "compila" y crea una imagen docker usando la informacion dada en el dockerfile
* docker build -t [que queremos para la imagen] [ruta]
* docker run --rm -ti [nombre de la imagen] [comando incial] : esto inicia el contenerdo y con los parametros que tiene se levanta de forma interactiva y al cerrarlo se elimina automaticamente.
* docker images rm [id de la imagen o nombre de la imagen] : elimina una imagen
* docker stop [id de la imagen] : detiene la ejecucion de un contenedor (esto es necesario para poder eliminar la imagen)
* docker run -ti --rm -p[numero de puerto en pc]:[numero de puerto en conetendor] [nombre de la imagen]
* docker run -ti --rm -v [rutalocal]:[nombre del volumen en el contenedor] [nombre y tag de la imagen]: con el parametro -v podemos asignar un fichero local para guardar cosas del contenedor pese a que el mismo se pare o se elimine la imagen.
