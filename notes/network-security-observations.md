# Observaciones sobre seguridad y monitorización de red

# Introducción

Durante el laboratorio se pudo observar cómo gran parte de la información que circula dentro de una red puede analizarse fácilmente utilizando herramientas de captura de tráfico como Wireshark.

Esto permitió comprender mejor la importancia de la monitorización de red dentro de entornos defensivos y cómo el análisis de tráfico puede ayudar a detectar actividad sospechosa, errores de configuración o problemas relacionados con seguridad.

Además, el laboratorio ayudó a entender que muchas veces la información más relevante no aparece únicamente en el contenido de los paquetes, sino también en patrones de comportamiento, conexiones y metadatos de red.

---

# Visibilidad del tráfico

Una de las observaciones más importantes fue comprobar la enorme cantidad de información que puede obtenerse simplemente observando tráfico de red.

Incluso sin acceder directamente a sistemas concretos, es posible identificar:

- direcciones IP
- puertos utilizados
- protocolos
- servicios activos
- dominios consultados
- tiempos de conexión
- patrones de comunicación

Esto demuestra por qué la monitorización de tráfico resulta tan importante dentro de tareas defensivas y análisis de seguridad.

---

# Riesgos relacionados con tráfico no cifrado

Durante las pruebas relacionadas con HTTP se observó claramente cómo determinadas comunicaciones viajan en texto plano cuando no existe cifrado.

Esto significa que, dependiendo del entorno, un atacante con capacidad de monitorización podría visualizar información transmitida entre sistemas.

Aunque actualmente gran parte del tráfico utiliza HTTPS, sigue existiendo mucho tráfico interno o mal configurado que continúa siendo visible.

---

# Importancia de los filtros

Otra observación importante fue comprobar cómo el uso correcto de filtros dentro de Wireshark facilita enormemente el análisis de tráfico.

Sin filtros adecuados, la cantidad de paquetes puede resultar prácticamente imposible de analizar manualmente.

Aprender a filtrar correctamente permite centrarse únicamente en:

- protocolos concretos
- IPs específicas
- puertos
- streams TCP
- tráfico sospechoso

---

# Monitorización defensiva

El laboratorio también ayudó a comprender cómo herramientas de captura de tráfico forman parte importante de entornos Blue Team y monitorización defensiva.

El análisis de tráfico puede utilizarse para:

- detectar anomalías
- identificar conexiones sospechosas
- monitorizar actividad
- analizar incidentes
- revisar comunicaciones

Además, resulta especialmente útil durante investigaciones relacionadas con incidentes de seguridad o análisis forense de red.

---

# Limitaciones del análisis de tráfico

Aunque Wireshark proporciona muchísima información, también se observaron ciertas limitaciones.

Por ejemplo:

- tráfico cifrado
- paquetes incompletos
- pérdidas de captura
- volumen elevado de tráfico

Esto demuestra que la monitorización de red normalmente debe complementarse con otras herramientas y sistemas de seguridad.

---

# Seguridad en redes internas

Otra observación importante fue entender que las redes internas no siempre son entornos seguros.

Muchas veces existe la falsa sensación de que el tráfico interno no necesita protección, cuando realmente gran parte de los ataques y movimientos laterales ocurren precisamente dentro de redes locales.

Por ello resulta importante aplicar:

- segmentación
- monitorización
- cifrado
- control de accesos
- revisión continua

---

> [!TIP]
> Analizar tráfico de red no solo sirve para detectar ataques. También ayuda muchísimo a entender cómo funcionan realmente las aplicaciones, protocolos y comunicaciones dentro de una infraestructura.

---

# Conclusiones

El laboratorio permitió comprender mucho mejor la importancia de la monitorización de tráfico dentro de entornos defensivos y cómo herramientas como Wireshark pueden utilizarse para analizar comunicaciones de red de forma muy detallada.

Además, ayudó a reforzar conocimientos relacionados con protocolos, networking, Blue Team y análisis defensivo de comunicaciones dentro de redes TCP/IP.
