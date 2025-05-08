
# Detección de Neumonía con IA

Este proyecto utiliza una red neuronal convolucional (CNN) entrenada para predecir si una radiografía de tórax muestra signos de neumonía.

## 🧠 Modelo

- Entrenado en Google Colab
- Basado en una arquitectura CNN
- Entrenado con dataset de imágenes de tórax

## 🚀 Demo (API)

Incluye una API construida en Flask que permite hacer predicciones con una imagen subida por el usuario.

## 📁 Estructura del proyecto

proyecto_neumonia/
├── modelo_entrenamiento.ipynb
├── api_demo.ipynb
├── modelo/
│ └── modelo_neumonia.h5
├── requirements.txt
├── README.md
└── .gitignore

**Descripción de los archivos:**

- `modelo_entrenamiento.ipynb`: Entrenamiento del modelo.
- `api_demo.ipynb`: Interfaz de prueba con Flask.
- `modelo/modelo_neumonia.h5`: Modelo entrenado.
- `requirements.txt`: Dependencias del proyecto.
- `README.md`: Descripción del proyecto.
- `.gitignore`: Exclusiones de Git.

---

## 🔧 Instalación

Para instalar las dependencias, ejecuta:

```bash
pip install -r requirements.txt

🧪 Prueba
Copia el notebook api_demo.ipynb y ejecuta una celda para subir una imagen de rayos X. El modelo clasificará la imagen como "Neumonía" o "Normal".

👨‍💻 Autor
Proyecto desarrollado como parte de un proyecto educativo.

