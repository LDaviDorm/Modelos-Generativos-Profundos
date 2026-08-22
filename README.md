# Modelos Generativos Profundos: Creatividad Computacional

Este repositorio contiene las implementaciones, prácticas y proyectos desarrollados durante el semestre 2027-1 para la exploración de modelos generativos aplicados a la creatividad computacional.

## Objetivo
El enfoque principal de estos códigos es la experimentación con arquitecturas generativas profundas para la creación de contenido sintético y el análisis de sus espacios latentes.

## Tecnologías y Entorno
Los notebooks están desarrollados principalmente en Jupyter, estructurados para ejecutarse de manera local utilizando **Visual Studio Code**.

El ecosistema de desarrollo principal incluye:
* **Frameworks de Deep Learning:** PyTorch (con soporte CUDA) y TensorFlow / Keras.
* **Visualización e Interfaces web:** Matplotlib, TensorBoard, Gradio y Streamlit para la creación de prototipos interactivos.
* **Lenguaje base:** Python 3.11

### Configuración del entorno local
Para replicar el entorno de desarrollo y ejecutar las libretas sin conflictos de dependencias, se utiliza Conda. Ejecuta los siguientes comandos en tu terminal:

```bash
# Clonar el repositorio
git clone [https://github.com/LDaviDorm/mgp-creatividad-computacional.git](https://github.com/LDaviDorm/mgp-creatividad-computacional.git)
cd mgp-creatividad-computacional

# Crear el entorno a partir del archivo de configuración
conda env create -f environment.yml

# Activar el entorno
conda activate mgp_env

# Vincular el entorno con Jupyter para VS Code
python -m ipykernel install --user --name=mgp_env --display-name="MGP (Python 3.11 - GPU)"