```text
██╗    ██╗██╗██████╗ ███████╗███████╗██╗  ██╗
██║    ██║██║██╔══██╗██╔════╝██╔════╝██║  ██║
██║ █╗ ██║██║██████╔╝█████╗  ███████╗███████║
██║███╗██║██║██╔══██╗██╔══╝  ╚════██║██╔══██║
╚███╔███╔╝██║██║  ██║███████╗███████║██║  ██║
 ╚══╝╚══╝ ╚═╝╚═╝  ╚═╝╚══════╝╚══════╝╚═╝  ╚═╝

Network Traffic Analysis · Packet Inspection · Blue Team
```

# Network Traffic Analysis with Wireshark

![Wireshark](https://img.shields.io/badge/Wireshark-Network%20Analysis-blue)
![Linux](https://img.shields.io/badge/Linux-Ubuntu-orange)
![Networking](https://img.shields.io/badge/TCP%2FIP-Networking-red)
![Blue Team](https://img.shields.io/badge/Blue%20Team-Traffic%20Analysis-green)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)

Laboratorio orientado a captura y análisis de tráfico de red utilizando Wireshark y herramientas de sniffing para inspeccionar protocolos, paquetes y comunicaciones dentro de un entorno virtualizado.

---

> [!NOTE]
> Todas las capturas y pruebas realizadas durante el laboratorio se ejecutaron sobre un entorno controlado y virtualizado con fines educativos y de aprendizaje.

---

# Descripción del proyecto

Este laboratorio se centra en el análisis de tráfico de red mediante herramientas de captura de paquetes, principalmente Wireshark, con el objetivo de comprender cómo circula la información dentro de una red y cómo pueden identificarse protocolos, comunicaciones y eventos relevantes desde una perspectiva defensiva.

Durante el proyecto se realizaron diferentes capturas de tráfico relacionadas con protocolos TCP/IP, peticiones HTTP, resolución DNS, tráfico ICMP y conexiones TCP, permitiendo analizar tanto la estructura de los paquetes como el flujo general de comunicación entre sistemas.

Además de aprender a utilizar Wireshark, una de las partes más importantes del laboratorio fue interpretar correctamente la información obtenida durante las capturas, comprendiendo cómo se identifican conexiones, direcciones IP, puertos, protocolos y posibles comportamientos sospechosos dentro del tráfico de red.

El entorno utilizado estuvo formado por varias máquinas virtuales conectadas mediante una red interna configurada desde VirtualBox, permitiendo generar tráfico controlado y analizarlo posteriormente desde la máquina encargada de monitorización.

---

# Objetivos del laboratorio

- Capturar tráfico de red utilizando Wireshark
- Analizar protocolos TCP/IP
- Inspeccionar paquetes y cabeceras
- Comprender el flujo de comunicaciones en red
- Identificar tráfico HTTP, DNS, ICMP y TCP
- Analizar direcciones IP y puertos
- Aprender técnicas básicas de sniffing
- Reforzar conocimientos de redes y monitorización

---

# Tecnologías y herramientas utilizadas

| Herramienta | Función |
|---|---|
| Wireshark | Captura y análisis de tráfico |
| Linux | Sistema utilizado durante las pruebas |
| Kali Linux | Generación de tráfico |
| Ubuntu Server | Sistema monitorizado |
| TCP/IP | Protocolos de red |
| VirtualBox | Virtualización del entorno |

---

# Arquitectura del laboratorio

| Máquina | Función |
|---|---|
| Kali Linux | Generación de tráfico |
| Ubuntu Server | Sistema monitorizado |
| Wireshark | Captura y análisis de paquetes |

El laboratorio se desarrolló dentro de una red interna virtualizada para permitir capturas controladas y análisis de tráfico sin afectar redes externas reales.

![Arquitectura del laboratorio](images/01-network-sniffer-topology.png)

---

# Análisis realizados

Durante el laboratorio se realizaron diferentes pruebas relacionadas con captura y análisis de tráfico:

- Captura de paquetes TCP
- Análisis de tráfico HTTP
- Resolución DNS
- Tráfico ICMP
- Identificación de direcciones IP
- Inspección de puertos
- Seguimiento de conexiones TCP
- Filtrado de tráfico mediante Wireshark

---

# Protocolos analizados

| Protocolo | Función |
|---|---|
| TCP | Comunicación orientada a conexión |
| UDP | Comunicación no orientada a conexión |
| ICMP | Diagnóstico y conectividad |
| DNS | Resolución de nombres |
| HTTP | Comunicación web |
| ARP | Resolución MAC/IP |

---

# Capturas del laboratorio

## Captura de paquetes en Wireshark

![Wireshark Capture](images/02-wireshark-capture.png)

---

## Análisis de tráfico HTTP

![HTTP Traffic](images/03-http-analysis.png)

---

## Resolución DNS

![DNS](images/04-dns-analysis.png)

---

## Seguimiento de conexiones TCP

![TCP Stream](images/06-tcp-stream.png)

---

# Resultados obtenidos

El laboratorio permitió comprender mejor cómo funciona la comunicación entre sistemas dentro de una red y cómo herramientas como Wireshark pueden utilizarse para inspeccionar tráfico y analizar protocolos en tiempo real.

Además, ayudó a reforzar conocimientos relacionados con:

- Redes TCP/IP
- Protocolos
- Captura de paquetes
- Análisis de tráfico
- Wireshark
- Monitorización
- Blue Team
- Networking
- Sniffing
- Diagnóstico de red

---

# Skills 

- Packet Analysis
- Wireshark
- Network Monitoring
- TCP/IP Analysis
- Traffic Inspection
- Protocol Analysis
- Blue Team Fundamentals
- Linux Networking
- Packet Capture
- Defensive Networking


---

# Documentación completa

La documentación técnica detallada se encuentra en:

[Ver documentación completa](docs/full-documentation.md)

---

> [!TIP]
> Analizar tráfico de red permite comprender cómo se comunican realmente los sistemas y ayuda a detectar comportamientos sospechosos, errores de configuración y actividad potencialmente maliciosa.

---

# Autor

Proyecto desarrollado como laboratorio práctico orientado a captura y análisis de tráfico de red utilizando Wireshark y herramientas de monitorización dentro de entornos Linux virtualizados.
