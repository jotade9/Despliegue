# Instalación de Bind9
Instalamos bind9  con los siguientes comandos: \n
sudo apt update
sudo apt install bind9 bind9utils bind9-doc -y


# Configuracion del archivo
Nos aseguramos de que las opciones forwarders estén configuradas con los DNS externos.
![img](https://github.com/jotade9/Despliegue/blob/main/Despliegue/DNS/Configuracion%20dle%20archivo.png)

# Configuración de la zona directa e inversa

## Zona directa
Editamos el archivo /etc/bind/named.conf.local para agregar la configuración de la zona directa e inversa. Además, agregamos la zona directa para ejemplo.com.

## Zona inversa
Agregamos la zona inversa (en este caso, para la IP 192.168.1.100)
![img](https://github.com/jotade9/Despliegue/blob/main/Despliegue/DNS/Zona%20directa%20e%20inversa.png)

# Creacion de los archivos de zona

## Zona directa
Creamos el archivo /etc/bind/db.ejemplo.com copiando la plantilla db.local, editamos el archivo /etc/bind/db.ejemplo.com y configuramos la zona directa.
![img](https://github.com/jotade9/Despliegue/blob/main/Despliegue/DNS/Zona%20directa.png)

## Zona inversa
Creamos el archivo /etc/bind/db.192, lo editamos y lo modificamos
![img](https://github.com/jotade9/Despliegue/blob/main/Despliegue/DNS/Zona%20inversa.png)

# Configuracion del archivo resolv.conf
Editamos el archivo /etc/resolv.conf y nos aseguramos que el econtenido indique el servidor DNS.
![img](https://github.com/jotade9/Despliegue/blob/main/Despliegue/DNS/Config%20archivo%20resolv.conf.png)

# Comprobar configuración
Comprobamos la configuración de bind 
![img](https://github.com/jotade9/Despliegue/blob/main/Despliegue/DNS/Comprobar%20y%20reiniciar.png)

## Prueba resolucion de nombres
Probamos la resolución de nombres con dig.
![img](https://github.com/jotade9/Despliegue/blob/main/Despliegue/DNS/Comprobacion%20resolucion%20de%20nombres.png)

## Comprobacion zona inversa
![img](https://github.com/jotade9/Despliegue/blob/main/Despliegue/DNS/Comprobamos%20zona%20inversa.png)

# Grabar los comandos con Asciinema
Para grabar necesitamos instalar asciinema con el siguiente comando: sudo apt install asciinema. Si queremos empezar a grabar utilizamos el comando asciinema rec.


