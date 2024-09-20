# **DNS**

# Resolución
Es el proceso mediante el cual se traduce un nombre de dominio legible por humanos(www.ubrique.es) en una dirección IP, que es la que realmente utilizan los dispositivos en internet para identificar y comunicarse entre sí.

# Nombre de dominio
Es la dirección que utilizas para acceder a un sitio web en Internet(www.ubrique.es). Se usa en lugar de la IP numérica(192.0.2.1) que es dificil de recordar.

# Niveles de dominio
Se refieren a la jerarquía de las partes que componen un nombre de dominio en Internet. Cada sección del dominio, separada por puntos, pertenece a un nivel en esta jerarquía. Estos niveles son fundamentales para organizar los nombres de dominio de manera lógica y escalable.

## Dominio de nivel superior(TLD).
Es la parte mas alta de la jerarquía de un nombre de dominio, situada a la derecha del todo. Hay dos tipos 		principales de TLD:

### TLD genéricos (gTLD)
Son los más comunes, como .com, .org, .net.
### TLD geográficos (ccTLD)
Representan a un país o región, como .es (España), .mx (México), .ar (Argentina).

## Dominio de Segundo Nivel (SLD)
Está justo a la izquierda del TLD y es el nombre principal que identifica a una organización, marca o persona. Es la parte del dominio que eliges cuando registras un sitio web. Ejemplo: En www.ejemplo.com, ejemplo es el dominio de segundo nivel.

## Subdominio (Dominio de Tercer Nivel)
Es opcional y se sitúa a la izquierda del dominio de segundo nivel. Se utiliza para dividir el sitio web en secciones o gestionar diferentes servicios bajo el mismo dominio. El subdominio más común es www, pero pueden ser personalizados, como blog.ejemplo.com o tienda.ejemplo.com. Ejemplo: En www.ejemplo.com, www es el subdominio, pero también puede ser otra cosa como blog.ejemplo.com.

## Dominio de Cuarto Nivel y posteriores
En algunos casos, se pueden usar dominios de cuarto nivel o más para organizar el sitio de manera aún más granular. Cada nuevo nivel añade más especificidad. Ejemplo: En ventas.europea.empresa.com, ventas sería el subdominio de cuarto nivel, europea el tercero, empresa el segundo nivel y .com el TLD.

Ejemplo completo:
Tercer nivel: www
Segundo nivel: ejemplo
Primer nivel (TLD): .com
	
# Zonas de busqueda
Es un término que hace referencia a una parte específica del espacio de nombres de dominio que es administrada por un servidor DNS autoritativo. Una zona define un grupo de nombres de dominio (junto con sus correspondientes registros de recursos) que están bajo el control de una misma entidad o servidor.

## Zona de búsqueda directa.
Asocia nombres de dominio con direcciones IP.
## Zona de búsqueda inversa
Asocia direcciones IP con nombres de dominio.
## Las zonas son administradas por servidores DNS autoritativos que contienen los registros DNS relevantes para la resolución de los nombres dentro de esa zona.

# Tipos de servidores
Cada servidor está diseñado para un servicio o función específica dentro de una red o en Internet.
## Servidor DNS
Traduce nombres de dominio a direcciones IP.
## Servidor Web
Aloja y entrega sitios web.
## Servidor de Archivos
Almacena y gestiona archivos.
## Servidor de Correo
Maneja el envío y recepción de correos electrónicos.
## Servidor de Base de Datos
Almacena y gestiona bases de datos.
## Servidor Proxy
Actúa como intermediario para mejorar seguridad o rendimiento.
## Servidor de Aplicaciones
Ejecuta aplicaciones empresariales o software.
## Servidor FTP
Facilita la transferencia de archivos mediante FTP.
## Servidor DHCP
Asigna automáticamente direcciones IP en redes locales.
## Servidor de Juegos
Permite partidas multijugador en línea.
## Servidor de Virtualización
Ejecuta múltiples máquinas virtuales en un solo equipo.
## Servidor de Medios
Almacena y distribuye contenido multimedia.
## Servidor de Impresión
Gestiona trabajos de impresión en una red.
## Servidor de Mensajería
Facilita el envío y recepción de mensajes en tiempo real.
## Servidor de Seguridad
Protege la red (firewall) o permite conexiones seguras (VPN).
## Servidor NTP
Sincroniza la hora en dispositivos de la red.

# Registros
Estos registros permiten la resolución y funcionamiento de los dominios en Internet.
## A (Address Record)
Asocia un dominio con una dirección IPv4.
## AAAA
Asocia un dominio con una dirección IPv6.
## CNAME (Canonical Name)
Redirige un dominio a otro dominio.
## MX (Mail Exchange)
Especifica los servidores de correo para un dominio.
## PTR (Pointer Record)
Utilizado para la resolución inversa (IP a nombre de dominio).
## NS (Name Server)
Indica los servidores DNS autoritativos de un dominio.
## TXT
Almacena texto útil para diversos propósitos, como verificaciones de seguridad (por ejemplo, SPF, DKIM).
## SOA (Start of Authority)
Proporciona información sobre la zona DNS y el servidor principal responsable.


# Funcionamiento
## Consulta recursiva
 El servidor DNS se encarga de todo el proceso de resolución y le devuelve la respuesta final al cliente.
## Consulta iterativa
El cliente interactúa con varios servidores DNS hasta obtener la respuesta final, siguiendo una cadena de referencias.
