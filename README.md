# iaupb_examen_06

Repositorio del trabajo de experimentación con YOLOv8 para detección de objetos sobre una imagen de prueba.

El notebook principal, [iaupb_examen_06_yolo.ipynb](iaupb_examen_06_yolo.ipynb), carga un modelo preentrenado de Ultralytics, ejecuta inferencias con distintas configuraciones de confianza y compara los resultados mediante tablas, gráficas y una visualización final de las detecciones.

## Objetivo

Evaluar cómo cambian las detecciones al variar el umbral de confianza manteniendo fijo el valor de IoU. El experimento compara tres configuraciones:

- Conservadora: `0.50`
- Balanceada: `0.25`
- Agresiva: `0.15`

## Contenido

- Carga de dependencias y librerías de visión por computador.
- Inicialización del modelo `yolov8n.pt`.
- Lectura de la imagen de entrada.
- Ejecución de inferencias con diferentes configuraciones.
- Cálculo y comparación de métricas de detección.
- Gráficas y panel visual con la imagen original y las imágenes anotadas.

## Requisitos

- Python 3.10 o superior.
- Jupyter Notebook o Google Colab.
- Paquetes principales:
	- `ultralytics`
	- `opencv-python`
	- `matplotlib`
	- `seaborn`
	- `pandas`
	- `numpy`

## Cómo ejecutar

1. Abre el notebook [iaupb_examen_06_yolo.ipynb](iaupb_examen_06_yolo.ipynb).
2. Instala las dependencias si aún no están disponibles.
3. Verifica la ruta de la imagen en la variable `IMAGE_PATH`.
4. Ejecuta las celdas en orden.
5. Revisa las tablas, las gráficas y la comparación visual de resultados.

## Resultado esperado

Al finalizar la ejecución, el notebook muestra:

- La cantidad total de objetos detectados por configuración.
- La confianza promedio de las detecciones.
- La distribución de las confianzas.
- Una comparación visual entre la imagen original y las versiones anotadas.

## Observaciones

- El notebook está orientado a un entorno tipo Colab, por lo que usa algunas utilidades específicas de ese entorno.
- Si cambias la imagen de entrada, ajusta también las rutas de salida o visualización que dependan de ella.