# Bitácora de Trabajo: TA-IND-01

   **13/11/2026**
- **Actividad:** Análisis y elección del sistema distribuido. Registro en el foro del SGA del tema "InfluxDB y comparación arquitectónica con Prometheus". Creación del repositorio y estructuración de los archivos base del informe.
- **Problemas encontrados:** Dudas iniciales sobre cómo ejecutar el sistema para las capturas al no tener un entorno local preparado.
- **Solución:** Se decidió utilizar GitHub Codespaces para levantar la arquitectura en Docker y realizar el experimento en la nube, asegurando que se muestre el usuario en la terminal.
- **Tiempo dedicado:** 2 horas.



### 14/11/2026 - Día 2: Desarrollo Experimental y Argumentación en LaTeX
* **Redacción del Marco Teórico (LaTeX):** Se desarrollaron las secciones críticas del informe en el archivo `main.tex`, detallando las Transparencias de Distribución de InfluxDB, su postura frente al Teorema CAP (y PACELC), los modelos de comunicación orientados a eventos (*Push*) y la comparación arquitectónica con Prometheus. Se incluyeron ejemplos del entorno local (SGA de la UTEQ y transferencias bancarias).
* **Consolidación Bibliográfica:** Se incorporaron fuentes verificadas de nivel académico e informes de incidentes reales en el archivo `referencias.bib` utilizando formato IEEE. Se tomaron capturas de evidencia de lectura de los artículos seleccionados (Anexo B).
* **Ejecución de Experimento Técnico (Dimensión 3):** Se levantó un entorno efímero en GitHub Codespaces utilizando contenedores Docker. Se simuló el modelo *Push* enviando métricas asincrónicas a la API HTTP (puerto 8086) y se forzó la interrupción del nodo de datos para comprobar empíricamente el comportamiento de disponibilidad (AP) y partición de red documentado en el marco teórico. Las evidencias (4 capturas y comandos ejecutados) se agregaron al repositorio.
