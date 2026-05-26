# Inspección de paquetes y cabeceras

# Introducción

Una de las partes más importantes del laboratorio consistió en analizar directamente los paquetes capturados mediante Wireshark para comprender cómo se estructura realmente la información transmitida dentro de una red.

El análisis de cabeceras permitió identificar información relacionada con protocolos, direcciones IP, puertos, flags y contenido transmitido entre sistemas.

---

# Capas analizadas

Durante las capturas se revisaron diferentes capas del modelo de red:

- Ethernet
- IP
- TCP
- UDP
- DNS
- HTTP
- ICMP

Wireshark permitió visualizar cada una de estas capas de forma detallada dentro de los paquetes capturados.

---

# Información observada

Entre los principales datos analizados se encontraron:

- IP origen y destino
- puertos
- protocolo utilizado
- longitud de paquetes
- flags TCP
- payloads
- secuencias
- tiempos

Esto ayudó especialmente a comprender cómo circula realmente la información dentro de la red.

---

# Payloads y contenido

En determinadas pruebas también fue posible visualizar contenido transmitido dentro de paquetes HTTP no cifrados.

Esto permitió entender cómo el tráfico sin cifrar puede exponer información sensible si es capturado dentro de la red.

---

# Importancia del análisis de paquetes

La inspección de paquetes resulta especialmente útil dentro de:

- monitorización defensiva
- troubleshooting
- análisis forense
- detección de anomalías
- revisión de protocolos

Además ayuda muchísimo a comprender cómo funcionan realmente las comunicaciones a nivel técnico.

---

# Conclusiones

La inspección de paquetes realizada durante el laboratorio permitió reforzar conocimientos relacionados con protocolos, networking y análisis de tráfico utilizando Wireshark como herramienta principal de monitorización.
