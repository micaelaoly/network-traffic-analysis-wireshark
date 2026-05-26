# Filtros utilizados en Wireshark

# Introducción

Durante el laboratorio se utilizaron diferentes filtros dentro de Wireshark con el objetivo de facilitar el análisis de tráfico y aislar únicamente los paquetes relevantes para cada prueba realizada.

Wireshark genera una enorme cantidad de información durante una captura, por lo que aprender a utilizar filtros correctamente resulta fundamental para poder interpretar el tráfico de forma eficiente y localizar rápidamente comunicaciones específicas dentro de la red.

---

# Filtros básicos utilizados

Uno de los filtros más utilizados durante el laboratorio fue:

```txt
icmp
```

Este filtro permitió visualizar únicamente tráfico ICMP relacionado principalmente con pruebas realizadas mediante `ping`.

También se utilizaron filtros relacionados con tráfico DNS:

```txt
dns
```

y tráfico HTTP:

```txt
http
```

El objetivo fue separar cada tipo de comunicación y analizar los protocolos de forma individual.

---

# Filtrado por dirección IP

Otra parte importante del laboratorio consistió en filtrar tráfico según direcciones IP concretas.

Ejemplo utilizado:

```txt
ip.addr == 192.168.56.10
```

Esto permitió visualizar únicamente paquetes relacionados con una máquina específica dentro del laboratorio.

También se utilizaron filtros más concretos relacionados con origen y destino:

```txt
ip.src == 192.168.56.10
```

```txt
ip.dst == 192.168.56.20
```

---

# Filtrado por puertos

Durante las pruebas relacionadas con tráfico TCP y HTTP también se utilizaron filtros orientados a puertos específicos.

Ejemplo:

```txt
tcp.port == 80
```

y:

```txt
tcp.port == 443
```

Esto ayudó especialmente a identificar comunicaciones web y analizar conexiones concretas dentro de la captura.

---

# Filtrado de tráfico TCP

Para visualizar únicamente tráfico TCP se utilizó:

```txt
tcp
```

Posteriormente se analizaron flags, streams y sesiones relacionadas con conexiones TCP activas.

---

# Seguimiento de streams

Una de las funciones más útiles utilizadas durante el laboratorio fue:

```txt
Follow TCP Stream
```

Esta funcionalidad permitió reconstruir conversaciones completas entre sistemas y visualizar el intercambio de información dentro de determinadas conexiones.

---

# Importancia de los filtros

La utilización correcta de filtros permitió reducir considerablemente la cantidad de tráfico visible y facilitar el análisis manual de paquetes.

Además, ayudó a comprender cómo herramientas de monitorización pueden utilizarse para detectar:

- tráfico sospechoso
- protocolos concretos
- conexiones específicas
- patrones de comunicación

---

# Conclusiones

El uso de filtros dentro de Wireshark resultó fundamental para analizar correctamente el tráfico capturado y comprender mucho mejor el comportamiento de las comunicaciones dentro de la red.
