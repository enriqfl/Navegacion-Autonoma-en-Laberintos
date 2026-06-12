# Navegación Autónoma en Laberintos (DFS)

Este repositorio contiene la implementación en Python de un agente inteligente diseñado para resolver laberintos generados procedimentalmente, utilizando el algoritmo de **Búsqueda en Grafo Primero en Profundidad (DFS)**. 

El proyecto incluye tanto el Notebook de Python con las visualizaciones interactivas como el reporte técnico formal en formato LaTeX.

## Estructura del Repositorio

* **`Notebook/`**: Contiene la implementación del algoritmo y la generación del entorno.
  * `Agente.ipynb`: Libreta principal de Jupyter con el código de generación del laberinto, la lógica del agente DFS y la animación paso a paso usando `matplotlib`.
  * `laberinto.gif`: Animación exportada que muestra el recorrido y la toma de decisiones del agente.
* **`Reporte/`**: Código fuente en LaTeX del documento técnico estructurado.
  * `main.tex`: Archivo principal del documento.
  * `main.pdf`: Reporte final compilado.
  * `img/`: Gráficos y capturas de la convergencia espacial extraídos del notebook.
  * `library.bib`: Referencias bibliográficas.

## Características del Algoritmo

1. **Generación Procedimental:** El laberinto estático se construye mediante *Randomized DFS*, garantizando que exista al menos una ruta válida hacia la meta.
2. **Exploración Sistemática:** El agente utiliza una pila (LIFO) para expandir los nodos más profundos de la frontera.
3. **Memoria de Estados:** Se implementó un control riguroso de nodos visitados para evitar bucles infinitos y retrocesos redundantes (*backtracking* eficiente).

## Uso y Reproducción

Para ejecutar el código localmente, asegúrate de contar con Python 3 y las siguientes dependencias instaladas:

```bash
pip install numpy matplotlib

git clone https://github.com/enriqfl/Navegacion-Autonoma-en-Laberintos.git
```

Navega a la carpeta del notebook y ejecuta **`Agente.ipynb`** en tu entorno preferido (Jupyter Lab, VSCode, Google Colab).
