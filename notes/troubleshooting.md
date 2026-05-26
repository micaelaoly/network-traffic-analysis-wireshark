# Problemas encontrados durante el laboratorio

# Introducción

Durante el desarrollo del laboratorio aparecieron diferentes problemas relacionados principalmente con interfaces de red, captura de tráfico y configuración del entorno virtualizado.

Muchos de estos errores fueron especialmente útiles para comprender cómo funciona realmente el tráfico dentro de una red y qué factores pueden afectar a la captura correcta de paquetes.

Además, resolver estos problemas ayudó a reforzar conocimientos relacionados con redes, interfaces, protocolos y monitorización de tráfico.

---

# Problemas con interfaces de red

Uno de los errores más frecuentes apareció al seleccionar interfaces incorrectas dentro de Wireshark.

En algunos casos la herramienta mostraba múltiples adaptadores de red y las capturas no contenían tráfico relevante porque se estaba monitorizando una interfaz equivocada.

Para solucionar esto fue necesario comprobar previamente las interfaces disponibles mediante:

```bash
ip a
```

y verificar cuál correspondía realmente a la red interna utilizada durante el laboratorio.

---

# Capturas vacías o sin tráfico

Otro problema habitual fue iniciar capturas sin generar tráfico entre máquinas.

En determinadas ocasiones Wireshark permanecía aparentemente sin actividad simplemente porque no existían comunicaciones activas dentro de la red.

La solución consistió en generar tráfico manualmente utilizando:

- ping
- consultas DNS
- conexiones HTTP
- tráfico TCP

Esto permitió comprobar inmediatamente el funcionamiento correcto de las capturas.

---

# Problemas relacionados con permisos

En algunos sistemas Linux aparecieron restricciones relacionadas con permisos de captura.

Wireshark requiere privilegios específicos para acceder directamente a interfaces de red, por lo que en determinados momentos fue necesario ejecutar herramientas con permisos elevados o revisar configuraciones relacionadas con captura de paquetes.

---

# Problemas con filtros

Otra parte que generó bastantes errores fue la utilización incorrecta de filtros dentro de Wireshark.

Pequeños errores de sintaxis podían provocar:

- ausencia de resultados
- tráfico incompleto
- visualización incorrecta
- filtros demasiado restrictivos

Esto obligó a revisar cuidadosamente expresiones relacionadas con:

- protocolos
- direcciones IP
- puertos
- streams TCP

---

# Problemas de conectividad

También aparecieron problemas relacionados con conectividad entre las máquinas virtuales.

En algunos casos determinadas pruebas no generaban tráfico porque las máquinas no podían comunicarse correctamente dentro de la red interna configurada en VirtualBox.

Para solucionarlo fue necesario revisar:

- configuración de adaptadores
- direcciones IP
- conectividad ICMP
- estado de interfaces

---

# Problemas al interpretar paquetes

Otra dificultad importante fue interpretar correctamente la información mostrada dentro de las capturas.

Wireshark muestra una enorme cantidad de datos relacionados con protocolos y cabeceras, por lo que inicialmente resultaba fácil perderse entre tanta información.

Conforme avanzó el laboratorio se empezó a entender mejor cómo identificar:

- IP origen y destino
- puertos
- flags TCP
- protocolos
- payloads
- secuencia de conexiones

---

# Problemas relacionados con tráfico cifrado

Durante algunas pruebas se observó que determinadas comunicaciones aparecían cifradas y no podían interpretarse completamente desde la captura.

Esto ayudó a comprender la diferencia entre:

- tráfico visible
- tráfico cifrado
- metadatos de conexión
- contenido real de paquetes

---

# Conclusiones

Los problemas encontrados durante el laboratorio ayudaron a comprender mucho mejor cómo funciona realmente la captura y análisis de tráfico dentro de redes TCP/IP.

Además de aprender a resolver errores técnicos, el proceso permitió desarrollar una visión más práctica sobre monitorización de red y análisis defensivo utilizando Wireshark.
