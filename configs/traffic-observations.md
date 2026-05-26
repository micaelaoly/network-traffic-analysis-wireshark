# Observaciones sobre tráfico de red

# Introducción

Durante el laboratorio se realizaron diferentes observaciones relacionadas con el comportamiento del tráfico dentro de la red virtualizada utilizada para las pruebas.

El análisis permitió comprender cómo distintos protocolos generan patrones específicos de comunicación y cómo herramientas como Wireshark facilitan enormemente la monitorización y análisis de paquetes.

---

# Tráfico generado

Las principales pruebas realizadas generaron tráfico relacionado con:

- ICMP
- DNS
- HTTP
- TCP
- ARP

Cada protocolo mostró comportamientos diferentes relacionados con tiempos, estructura de paquetes y flujo de comunicación.

---

# Comunicación entre sistemas

Una de las observaciones más interesantes fue comprobar cómo prácticamente cualquier interacción entre máquinas genera múltiples paquetes relacionados con diferentes protocolos.

Incluso acciones simples como realizar un ping o abrir una página web implican múltiples comunicaciones previas relacionadas con resolución DNS, ARP y establecimiento de conexiones TCP.

---

# Importancia de la monitorización

El laboratorio también permitió observar cómo el análisis de tráfico puede utilizarse para:

- identificar actividad
- detectar errores
- monitorizar conexiones
- revisar comportamiento de aplicaciones
- analizar incidencias

Esto demuestra por qué la monitorización de red resulta tan importante dentro de entornos Blue Team y seguridad defensiva.

---

# Tráfico cifrado y visible

Otra observación importante fue diferenciar entre tráfico visible y tráfico cifrado.

Aunque determinadas comunicaciones HTTPS protegen el contenido transmitido, siguen existiendo metadatos visibles relacionados con:

- IPs
- puertos
- tiempos
- protocolos
- tamaño de paquetes

Esto demuestra que incluso el tráfico cifrado sigue proporcionando información útil para análisis de red.

---

# Conclusiones

Las observaciones realizadas durante el laboratorio ayudaron a comprender mucho mejor cómo funcionan realmente las comunicaciones dentro de redes TCP/IP y cómo herramientas de captura permiten analizar tráfico de forma detallada desde una perspectiva defensiva.
