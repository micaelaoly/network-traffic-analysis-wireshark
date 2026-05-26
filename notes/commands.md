# Comandos utilizados durante el laboratorio

# Introducción

Durante el laboratorio se utilizaron diferentes herramientas y comandos relacionados con captura de tráfico, análisis de paquetes y monitorización básica de red utilizando Wireshark y utilidades nativas de Linux.

Además de aprender el funcionamiento de cada comando, una de las partes más importantes fue comprender cómo interpretar correctamente la información obtenida durante las capturas y cómo relacionarla con el comportamiento real de la red.

La combinación entre tráfico generado desde Kali Linux y análisis posterior desde Wireshark permitió entender mucho mejor cómo funcionan realmente las comunicaciones TCP/IP a nivel de paquetes.

---

# Comandos de conectividad

Para generar tráfico básico dentro de la red se utilizaron herramientas como:

```bash
ping
```

Ejemplo:

```bash
ping 192.168.56.20
```

Este tipo de tráfico permitió analizar paquetes ICMP y comprobar conectividad entre las máquinas virtuales del laboratorio.

También se realizaron pruebas utilizando:

```bash
traceroute
```

con el objetivo de observar el recorrido de paquetes y comprender mejor el comportamiento del tráfico en red.

---

# Identificación de interfaces de red

Antes de comenzar las capturas fue necesario identificar correctamente las interfaces disponibles dentro del sistema.

Para ello se utilizó:

```bash
ip a
```

Este comando permitió visualizar:

- interfaces activas
- direcciones IP
- máscaras de red
- estado de conexión

Identificar correctamente la interfaz fue especialmente importante para evitar realizar capturas sobre adaptadores incorrectos.

---

# Captura de tráfico

Aunque la mayor parte del análisis se realizó desde la interfaz gráfica de Wireshark, también se trabajó con herramientas de terminal como:

```bash
tcpdump
```

Ejemplo:

```bash
sudo tcpdump -i eth0
```

Esto permitió comprender mejor cómo funcionan las capturas de tráfico incluso sin entorno gráfico.

---

# Resolución DNS

Para generar tráfico relacionado con resolución de nombres se utilizaron herramientas como:

```bash
nslookup
```

y:

```bash
dig
```

Estas pruebas ayudaron a analizar:

- consultas DNS
- respuestas DNS
- resolución de dominios
- comportamiento del protocolo

---

# Comandos de análisis de red

También se realizaron comprobaciones utilizando:

```bash
netstat
```

y:

```bash
ss
```

El objetivo fue observar conexiones activas, puertos abiertos y sesiones de red establecidas dentro del laboratorio.

---

# Filtros utilizados en Wireshark

Durante el análisis se aplicaron diferentes filtros para facilitar la visualización del tráfico.

Algunos de los más utilizados fueron:

```txt
http
```

```txt
dns
```

```txt
icmp
```

```txt
tcp
```

```txt
ip.addr == 192.168.56.10
```

```txt
tcp.port == 80
```

La utilización de filtros permitió aislar tráfico específico y comprender mucho mejor el funcionamiento individual de cada protocolo.

---

# Seguimiento de streams TCP

Una de las funciones más útiles trabajadas durante el laboratorio fue:

```txt
Follow TCP Stream
```

Esta opción permitió reconstruir conversaciones completas entre sistemas y visualizar el contenido intercambiado durante determinadas conexiones.

---

# Análisis de paquetes

Durante el laboratorio también se inspeccionaron cabeceras de paquetes relacionadas con:

- IP
- TCP
- UDP
- DNS
- HTTP
- ICMP

Esto ayudó especialmente a comprender cómo se estructura realmente la comunicación entre sistemas a nivel de red.

---

# Conclusiones

Los comandos y herramientas utilizados durante el laboratorio permitieron comprender mucho mejor cómo se generan, transmiten y analizan los paquetes dentro de una red TCP/IP.

Además de aprender a utilizar Wireshark, la parte más importante fue interpretar correctamente el tráfico capturado y relacionarlo con el comportamiento real de las comunicaciones entre sistemas.
