# Análisis de protocolos de red

# Introducción

Durante el laboratorio se analizaron diferentes protocolos de red con el objetivo de comprender cómo funcionan realmente las comunicaciones dentro de una infraestructura TCP/IP.

El análisis se realizó utilizando Wireshark para capturar e inspeccionar paquetes relacionados con protocolos como TCP, UDP, ICMP, DNS, HTTP y ARP.

Además de identificar los protocolos utilizados, también se revisaron cabeceras, comportamiento de conexiones y flujo de comunicación entre sistemas.

---

# Protocolo TCP

TCP fue uno de los protocolos más analizados durante el laboratorio.

Este protocolo proporciona comunicación orientada a conexión y garantiza entrega correcta de datos entre sistemas.

Durante las capturas se analizaron especialmente:

- handshake de tres vías
- flags TCP
- secuencias
- acknowledgements
- cierre de sesiones

También se observó cómo Wireshark permite seguir conversaciones completas mediante streams TCP.

---

# Protocolo UDP

UDP se analizó principalmente durante tráfico relacionado con DNS.

A diferencia de TCP, UDP no establece conexiones ni garantiza entrega de paquetes, lo que permite comunicaciones más rápidas pero menos fiables.

Esto resulta útil especialmente en servicios donde la velocidad tiene prioridad sobre la confirmación de entrega.

---

# Protocolo ICMP

ICMP apareció principalmente durante pruebas realizadas mediante `ping`.

Se analizaron:

- Echo Request
- Echo Reply
- tiempos de respuesta
- conectividad entre sistemas

Este protocolo se utiliza principalmente para diagnóstico y comprobaciones de red.

---

# Protocolo DNS

DNS permitió observar cómo los sistemas resuelven nombres de dominio antes de establecer conexiones.

Durante el análisis se revisaron:

- consultas DNS
- respuestas
- dominios solicitados
- servidores utilizados

Esto ayudó a comprender mejor cómo funciona la navegación y resolución de nombres dentro de redes TCP/IP.

---

# Protocolo HTTP

También se realizaron pruebas relacionadas con tráfico HTTP.

El análisis permitió observar:

- peticiones GET
- respuestas del servidor
- cabeceras HTTP
- contenido transmitido

Además, ayudó a entender cómo el tráfico HTTP puede visualizarse en texto claro cuando no existe cifrado.

---

# Protocolo ARP

ARP apareció durante comunicaciones dentro de la red local.

Este protocolo permite asociar direcciones IP con direcciones MAC para facilitar comunicaciones Ethernet dentro de redes internas.

Aunque normalmente pasa desapercibido, resulta fundamental para el funcionamiento correcto de las comunicaciones locales.

---

# Conclusiones

El análisis de protocolos permitió comprender mucho mejor cómo se estructuran las comunicaciones dentro de una red y cómo herramientas como Wireshark pueden utilizarse para inspeccionar tráfico de forma detallada.
