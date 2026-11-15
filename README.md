# TA-IND-01: Análisis Crítico de InfluxDB vs Prometheus

**Universidad Técnica Estatal de Quevedo (UTEQ)**  
**Asignatura:** Sistemas Distribuidos  
**Estudiante:** Cesar Abrahan Macias Vasquez (@CesarMacias007)  

Este repositorio contiene el informe académico individual y las evidencias experimentales sobre la arquitectura distribuida de InfluxDB, su modelo de comunicación *Push*, su comportamiento frente al Teorema CAP (y PACELC), y una comparación técnica de bajo nivel con Prometheus.

---

##  Video de Sustentación
Puedes revisar la explicación de la arquitectura y la demostración del experimento de caída de nodo en el siguiente enlace:

 **el video se esta elaborando**

---

##  Contenido del Repositorio
- `main.tex` y `referencias.bib`: Código fuente en LaTeX del informe y su bibliografía IEEE.
- `BITACORA.md`: Registro detallado de las actividades realizadas durante los días de trabajo.
- `comandos_experimento.txt`: Registro del despliegue efímero en Docker y pruebas HTTP (*cURL*) realizadas en Codespaces.
- `*.png / *.jpeg`: Evidencias visuales de la arquitectura, fuentes académicas leídas (Anexo B) y capturas de la terminal (Anexo C).

##  Instrucciones de Compilación (LaTeX)
Para compilar este documento y regenerar el PDF correctamente con sus referencias IEEE, se debe ejecutar la siguiente secuencia de comandos en la terminal (recomendado usar GitHub Codespaces o Overleaf):

```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
