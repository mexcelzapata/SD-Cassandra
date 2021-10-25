# SD-Cassandra
Para poder instalar y dejar arriba el sistema de base de datos no SQL "Casandra" en un entorno Linux es necesario poder instalar las siguientes dependencias:

## Paso 1: Instalación de Dependencias
###Instalar Java OpendJDK
Actualizar el repositorio de paquetes del SO:

```
sudo apt update
```
Instalar OpenJDK 8:

```
sudo apt install openjdk-8-jdk -y
```

Verificamos la version de Java.

```
Java -version
```
>Openjdk version "1.8.0_252"

### Instalar paquete de transporte APT
Para permitir el acceso a los repositorios mediante HTTPS.
```
sudo apt install apt-transport-https
```

## Paso 2: Instalacion de Apache Cassandra e importar la clave GPG

### Agregar a la lista de fuentes el repositorio de Cassandra
```
sudo sh -c 'echo "deb http://www.apache.org/dist/cassandra/debian 40x main" > /etc/apt/sources.list.d/cassandra.list'
```

### Extraer Cassandra a traves de la URL
```
wget -q -O - https://www.apache.org/dist/cassandra/KEYS | sudo apt-key add -
```


## Paso 3: Instalacion de Apache Cassandra

Actualizar el repositorio de paquetes del SO:
```
sudo apt update
```

Instalamos Cassandra con el comando: 

```
sudo apt install Cassandra

```










