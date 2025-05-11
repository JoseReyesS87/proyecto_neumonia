# 🩺 Detección de Neumonía con Inteligencia Artificial

Este proyecto implementa un modelo de red neuronal convolucional (CNN) capaz de detectar signos de neumonía en radiografías de tórax. Utiliza aprendizaje profundo para asistir en el diagnóstico médico a partir de imágenes.

---

## 🧠 Modelo

- Entrenado en Google Colab con TensorFlow y Keras.
- Basado en una arquitectura **CNN personalizada**.
- Utiliza un conjunto de **9.341 imágenes de rayos X** de tórax divididas entre clases "Normal" y "Neumonía".
- Datos divididos en entrenamiento, validación y test.
- Evaluado con métricas como **precisión, recall y matriz de confusión**.

---

## 📊 Dataset

El modelo fue entrenado con el dataset [Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia), que contiene:

- **5.216 imágenes de entrenamiento**
- **624 imágenes de validación**
- **1.624 imágenes de prueba**

Las imágenes están clasificadas en dos clases:

- **NORMAL**
- **PNEUMONIA**

---

## 🚀 Demo: API con Flask

Se incluye una API sencilla, construida con Flask, que permite cargar imágenes de rayos X y obtener una predicción en tiempo real.

- El demo está contenido en el notebook `api_demo.ipynb`.
- El usuario puede cargar una imagen y recibir como salida la predicción: **"Neumonía" o "Normal"**.
- Todo el codigo esta pensado para ejecutarlo de forma gratuita mediante Ngrok y Google Colab

---


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

🧪 Prueba el modelo
Puedes probar el modelo con Google Colab desde el notebook api_demo.ipynb:

Ejecuta el notebook y visita el link entregado con Flask, veras una pagina web en la cual puedes subir tu radiografia de Torax y enviarla al modelo.

Recibirás la clasificación: Neumonía o Normal.

💡 Posibles mejoras futuras
Entrenamiento con más imágenes y data augmentation.

Despliegue de la API en servicios como Render o HuggingFace Spaces.

Interfaz web amigable para uso médico.

👨‍💻 Autor
Proyecto desarrollado por Jose Reyes como parte de una iniciativa educativa para explorar aplicaciones prácticas de redes neuronales.

📜 Licencia
Este proyecto se publica con fines educativos. Revisa las condiciones del dataset original en su página de Kaggle (https://colab.research.google.com/drive/1UWipQ0e9RcLijCu3zj2E61MHK4o3jVol#scrollTo=l5Voln97gY_B&line=91&uniqifier=1)

