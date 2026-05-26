# Observaciones sobre protocolos de red

# Introducción

Durante el laboratorio se analizaron diferentes protocolos de red con el objetivo de comprender cómo se comunican realmente los sistemas dentro de una infraestructura TCP/IP.

Una de las partes más interesantes fue observar cómo cada protocolo tiene una función específica y cómo todos trabajan conjuntamente para permitir comunicaciones entre dispositivos, resolución de nombres y transferencia de información.

El análisis realizado mediante Wireshark permitió visualizar el comportamiento real de estos protocolos a nivel de paquetes y cabeceras.

---

# Protocolo TCP

TCP fue uno de los protocolos más analizados durante el laboratorio.

Se observó especialmente:

- establecimiento de conexiones
- handshake de tres vías
- flags TCP
- retransmisiones
- cierre de sesiones

El seguimiento de streams TCP permitió visualizar conversaciones completas entre sistemas y comprender mucho mejor cómo funciona la comunicación orientada a conexión.

También se analizaron aspectos relacionados con:

- puertos
- secuencias
- acknowledgements
- control de flujo

---

# Protocolo ICMP

El tráfico ICMP apareció principalmente durante pruebas realizadas con `ping`.

Este protocolo permitió observar:

- solicitudes Echo Request
- respuestas Echo Reply
- tiempos de respuesta
- conectividad entre máquinas

Aunque ICMP no se utiliza para transferencia de información como TCP o UDP, resulta muy importante para diagnóstico y monitorización de red.

---

# Resolución DNS

Otra parte muy importante del laboratorio fue el análisis de tráfico DNS.

Las capturas permitieron observar cómo los sistemas realizan consultas para resolver nombres de dominio antes de establecer conexiones.

Se analizaron especialmente:

- consultas DNS
- respuestas DNS
- dominios solicitados
- servidores utilizados
- tiempos de resolución

Esto ayudó a comprender mejor la relación entre navegación y resolución de nombres dentro de una red.

---

# Protocolo HTTP

También se realizaron pruebas relacionadas con tráfico HTTP.

El análisis permitió observar:

- peticiones GET
- respuestas del servidor
- cabeceras HTTP
- contenido transmitido
- métodos de comunicación web

Una de las partes más interesantes fue comprobar cómo HTTP transmite información en texto claro cuando no existe cifrado.

---

# Protocolo ARP

Durante las capturas también apareció tráfico ARP relacionado con resolución de direcciones MAC.

Este protocolo se encarga de asociar direcciones IP con direcciones físicas dentro de redes locales.

Aunque normalmente pasa desapercibido, resulta fundamental para el funcionamiento correcto de las comunicaciones Ethernet.

---

# Importancia del análisis de protocolos

Analizar protocolos permitió comprender mucho mejor cómo funcionan realmente las redes más allá de la teoría.

Observar paquetes reales ayuda especialmente a entender:

- flujo de comunicaciones
- intercambio de información
- establecimiento de conexiones
- comportamiento de aplicaciones
- monitorización defensiva

Además, este tipo de análisis resulta muy útil dentro de tareas relacionadas con:

- Blue Team
- troubleshooting
- análisis forense
- detección de anomalías
- monitorización de red

---

# Conclusiones

El análisis de protocolos realizado durante el laboratorio permitió comprender mucho mejor cómo se estructuran las comunicaciones dentro de redes TCP/IP y cómo herramientas como Wireshark pueden utilizarse para inspeccionar tráfico de forma detallada.

Además, ayudó a reforzar conocimientos relacionados con networking, monitorización y análisis defensivo de comunicaciones.
