# 💬 Análisis de Sentimiento con RNN, LSTM y Exploración de Transformer

Este proyecto aplica técnicas de procesamiento de lenguaje natural (NLP) y aprendizaje profundo para clasificar sentimientos en tweets. El enfoque principal está en comparar dos arquitecturas clásicas: **RNN (Recurrent Neural Network)** y **LSTM (Long Short-Term Memory)** usando el dataset **Sentiment140**.

Adicionalmente, se incluye una implementación educativa de un **Transformer básico** en PyTorch como experimento conceptual, sin fines comparativos directos.

---

## 📊 Dataset

Se utiliza el dataset [Sentiment140](http://help.sentiment140.com/), que contiene 1.6 millones de tweets etiquetados como positivos o negativos.

El dataset se descarga automáticamente dentro del notebook usando `wget`, por lo que **no es necesario subirlo manualmente**.

> ⚠️ En caso de falla con el enlace, puedes obtenerlo desde [Kaggle](https://www.kaggle.com/datasets/kazanova/sentiment140).

---

## 🧠 Modelos Desarrollados

### 🔁 RNN vs LSTM (Keras, TensorFlow)
- Entrenamiento de ambas arquitecturas para clasificación binaria
- Visualización y análisis de precisión, F1-score y pérdida
- Comparación directa entre modelos para determinar el más efectivo

### 🧪 Transformer (PyTorch) — *Exploración Conceptual*
- Implementación desde cero basada en el paper original de Vaswani et al.
- Explicación didáctica de codificación posicional, atención y estructura encoder
- No se compara directamente con RNN o LSTM en métricas

---

## 📈 Resultados: RNN vs LSTM

| Modelo     | Precisión | F1-Score | Tiempo de Entrenamiento | Tamaño del Modelo |
|------------|-----------|----------|--------------------------|-------------------|
| RNN        | 72.9%     | 0.72     | ~12 min                  | 24.8 MB           |
| LSTM       | 77.0%     | 0.77     | ~15 min                  | 27.2 MB           |

> ✅ Se eligió **LSTM** como modelo final por su mejor desempeño general y mayor estabilidad durante el entrenamiento.

---

## ⚙️ Tecnologías utilizadas

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white) ![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white) ![NLTK](https://img.shields.io/badge/NLTK-3776AB?style=for-the-badge&logo=python&logoColor=ffdd54) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)

[//]: # "- Python 3"
[//]: # "- TensorFlow/Keras"
[//]: # "- PyTorch"
[//]: # "- scikit-learn"
[//]: # "- NLTK"
[//]: # "- pandas, numpy, matplotlib"

---

## 📁 Estructura del Proyecto

```

sentiment-analysis-rnn-lstm-transformer/
│
├── notebooks/
│   ├── rnn_vs_lstm.ipynb             
│   └── transformer_exploration.ipynb 
│
├── models/
│   ├── rnn_model.keras
│   ├── lstm_model.keras
│   └── transformer_model.pth                           
│
├── requirements.txt
├── README.md
└── .gitignore

````

---

## 🚀 ¿Cómo ejecutar los notebooks?

1. Clona el repositorio:
```
   git clone https://github.com/tu_usuario/sentiment-analysis-rnn-lstm-transformer.git
   cd sentiment-analysis-rnn-lstm-transformer
```

2. Instala las dependencias:

```
   pip install -r requirements.txt
```

3. Abre y ejecuta los notebooks desde tu entorno favorito:

   * `notebooks/rnn_vs_lstm.ipynb` para la comparación principal
   * `notebooks/transformer_exploration.ipynb` para la arquitectura Transformer educativa

---

## 📄 Licencia

Este proyecto está bajo la licencia MIT.

---

## 👤 Autor

Desarrollado por Alexis Martínez.
Incluye aprendizaje profundo aplicado a NLP, análisis comparativo de modelos secuenciales y una exploración didáctica de la arquitectura Transformer.
