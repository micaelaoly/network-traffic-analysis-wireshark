# Análisis de tráfico TCP

# Introducción

Durante el laboratorio se realizaron diferentes pruebas relacionadas con tráfico TCP con el objetivo de comprender cómo funcionan realmente las conexiones orientadas a comunicación fiable dentro de redes TCP/IP.

Wireshark permitió observar el comportamiento completo de las conexiones, desde el establecimiento inicial hasta el cierre de la sesión.

---

# Handshake de tres vías

Una de las partes más importantes analizadas fue el establecimiento de conexiones mediante el handshake TCP.

Durante las capturas se observaron los paquetes:

- SYN
- SYN ACK
- ACK

Este intercambio inicial permite establecer correctamente la comunicación entre cliente y servidor antes de comenzar la transmisión de datos.

---

# Flags TCP

También se analizaron diferentes flags utilizadas por el protocolo TCP:

| Flag | Función |
|---|---|
| SYN | Inicio de conexión |
| ACK | Confirmación |
| FIN | Cierre de sesión |
| RST | Reinicio de conexión |
| PSH | Envío inmediato de datos |

El análisis de estas flags ayudó especialmente a comprender el estado de las conexiones durante las capturas.

---

# Puertos TCP

Durante las pruebas también se identificaron puertos utilizados por distintos servicios.

Ejemplos observados:

- 80 → HTTP
- 443 → HTTPS
- 22 → SSH
- 53 → DNS

Esto permitió relacionar protocolos y servicios con sus comunicaciones reales dentro de la red.

---

# Seguimiento de streams TCP

Wireshark permitió reconstruir conversaciones completas mediante:

```txt
Follow TCP Stream
```

Esta funcionalidad facilitó visualizar intercambios completos de información entre cliente y servidor.

---

# Retransmisiones y errores

Durante algunas pruebas también se observaron retransmisiones TCP y pequeños retrasos relacionados con conectividad o tiempos de respuesta.

Esto ayudó a comprender cómo TCP gestiona errores y garantiza entrega correcta de información.

---

# Conclusiones

El análisis de tráfico TCP permitió comprender mucho mejor cómo funcionan las conexiones orientadas a comunicación fiable y cómo Wireshark puede utilizarse para inspeccionar sesiones completas dentro de una red.
