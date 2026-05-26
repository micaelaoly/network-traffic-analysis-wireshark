# Análisis de tráfico DNS

# Introducción

Durante el laboratorio se analizaron consultas y respuestas DNS capturadas mediante Wireshark con el objetivo de comprender cómo funciona la resolución de nombres dentro de redes TCP/IP.

El protocolo DNS resulta fundamental porque permite traducir dominios legibles para humanos en direcciones IP utilizadas realmente por los sistemas.

---

# Funcionamiento de DNS

Antes de establecer conexiones con servidores web u otros servicios, los sistemas normalmente realizan consultas DNS para resolver el nombre solicitado.

Durante el laboratorio se observaron:

- consultas DNS
- respuestas DNS
- tiempos de resolución
- servidores utilizados

---

# Captura de consultas

Para generar tráfico DNS se realizaron pruebas utilizando:

```bash
nslookup
```

y navegación web básica.

Posteriormente se filtró el tráfico mediante:

```txt
dns
```

Esto permitió visualizar únicamente paquetes relacionados con resolución de nombres.

---

# Información observada

Durante las capturas se identificaron:

- dominios solicitados
- IPs devueltas
- tipo de consulta
- identificadores DNS
- tiempos de respuesta

El análisis permitió comprender mejor cómo funciona realmente la resolución de nombres dentro de Internet.

---

# Riesgos relacionados con DNS

También se comentó cómo determinadas consultas DNS pueden utilizarse para:

- monitorización
- análisis de actividad
- detección de comportamiento
- identificación de servicios utilizados

Por ello DNS resulta especialmente importante dentro de tareas defensivas y monitorización de red.

---

# Conclusiones

El análisis de tráfico DNS ayudó a comprender cómo los sistemas resuelven nombres antes de establecer comunicaciones y cómo este protocolo resulta clave dentro del funcionamiento normal de redes TCP/IP.
