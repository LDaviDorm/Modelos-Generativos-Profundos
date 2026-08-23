# Modelos Generativos Profundos: Creatividad Computacional

Este repositorio contiene las implementaciones, prácticas y proyectos desarrollados durante el semestre 2027-1 para la exploración de modelos generativos aplicados a la creatividad computacional.

## Objetivo
El enfoque principal de estos códigos es la experimentación con arquitecturas generativas profundas para la creación de contenido sintético y el análisis de sus espacios latentes.

## Tecnologías y Entorno
Los notebooks están desarrollados principalmente en Jupyter, estructurados para ejecutarse de manera local utilizando **Visual Studio Code**.

El ecosistema de desarrollo principal incluye:
* **Frameworks de Deep Learning:** PyTorch (con y sin soporte CUDA) y TensorFlow / Keras.
* **Visualización e Interfaces web:** Matplotlib, TensorBoard, Gradio y Streamlit para la creación de prototipos interactivos.
* **Lenguaje base:** Python 3.11

## Configuración del entorno local
Para replicar el entorno de desarrollo y manejar el código sin errores de dependencias al alternar entre la PC de escritorio con GPU y la laptop con CPU, se utilizan configuraciones separadas de Conda. 

Primero, clona el repositorio e ingresa a la carpeta:
```bash
git clone https://github.com/LDaviDorm/mgp-creatividad-computacional.git
cd mgp-creatividad-computacional
```

Luego, ejecuta los comandos correspondientes según el hardware de la máquina en uso:

### Opción A: Equipos sin GPU dedicada (Solo CPU - Laptop)
```bash
# Crear el entorno a partir del archivo de configuración
conda env create -f environment_cpu.yml
# Activar el entorno
conda activate mgp_env_cpu
# Vincular el entorno con Jupyter para VS Code
python -m ipykernel install --user --name=mgp_env_cpu --display-name="MGP (Python 3.11 - CPU)"
```

### Opción B: Equipos con GPU NVIDIA (Soporte CUDA - PC)
```bash
# Crear el entorno a partir del archivo de configuración
conda env create -f environment_gpu.yml
# Activar el entorno
conda activate mgp_env_gpu
# Vincular el entorno con Jupyter para VS Code
python -m ipykernel install --user --name=mgp_env_gpu --display-name="MGP (Python 3.11 - GPU)"
```