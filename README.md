# 🧠 NVIDIA AI Workshops

Repositorio de aprendizaje intensivo de 3 días en **Deep Learning** y **Machine Learning**, desarrollado en el marco de los talleres de NVIDIA. Cada día aborda un conjunto de técnicas y arquitecturas progresivamente más avanzadas, desde clasificación de imágenes hasta modelos generativos de difusión.

---

## 📅 Estructura del Programa

### Día 1 — Fundamentos de Deep Learning & Visión por Computador

Introducción a redes neuronales convolucionales (CNN) aplicadas a la clasificación de imágenes.

**Temas cubiertos:**
- Construcción de bloques convolucionales personalizados (`MyConvBlock`) con `Conv2d`, `BatchNorm`, `ReLU`, `Dropout` y `MaxPool`
- Ciclos de entrenamiento y validación con PyTorch
- Data augmentation mediante transformaciones aleatorias (`random_trans`)
- Métricas de evaluación: pérdida y precisión por lote

**Tecnologías:** PyTorch, torchvision

---

### Día 2 — Detección de Anomalías: XGBoost & GANs

Aplicación de modelos supervisados y no supervisados para la detección de intrusiones y anomalías en redes.

**Temas cubiertos:**
- Preprocesamiento del dataset **KDD Cup** (codificación categórica, one-hot encoding, normalización)
- Árboles de decisión potenciados con **XGBoost** para clasificación de ataques de red
- Detección de anomalías con GANs en escenarios de datos desbalanceados
- Pipeline completo: `train_test_split`, `LabelEncoder`, serialización con `pickle`

**Tecnologías:** scikit-learn, XGBoost, pandas, numpy, PyTorch

---

### Día 3 — Modelos Generativos: Autoencoders, GANs & Difusión

Exploración de arquitecturas generativas para síntesis de datos y representaciones latentes, culminando con la técnica de difusión.

**Temas cubiertos:**
- Autoencoders variacionales (VAE) para aprendizaje de representaciones comprimidas
- Redes Generativas Antagónicas (GANs): entrenamiento del generador y el discriminador
- Técnica de **difusión** aplicada a modelos generativos para mejorar la calidad de las muestras
- Evaluación visual y cuantitativa de las imágenes generadas

**Tecnologías:** PyTorch, matplotlib, numpy

---

## 🗂️ Estructura del Repositorio

```
Nvidia-AI-Workshops/
├── notebooks/
│   ├── day1/                     # Notebooks: clasificación de imágenes con CNNs
│   ├── day2/                     # Notebooks: detección de anomalías (XGBoost & GANs)
│   └── day3/                     # Notebooks: modelos generativos y difusión
├── scripts/
│   ├── day 1/
│   │   └── utils.py              # Bloques CNN, entrenamiento y validación
│   └── day 3/
│       └── ...                   # Scripts de entrenamiento generativo
├── static/
│   ├── day3/                     # Resultados: imágenes generadas, proceso de difusión
│   └── images/                   # Imagenes: imagenes estaticas de cada notebook
├── requirements.txt
├── README.md
└── LICENSE
```

---

## 🖼️ Resultados

### Día 3 — Modelos Generativos & Difusión

#### Flores generadas

##### Epoca 5

![Epoca 5](/static/day%203/Diffusion%20Result%20(5%20Epoch).png)

##### Epoca 50

![Epoca 50](/static/day%203/Diffusion%20Result%20(50%20Epoch).png)

##### Epoca 100

![Epoca 100](/static/day%203/Diffusion%20Result%20(100%20Epoch).png)

---

## ⚙️ Requisitos

```bash
pip install -r requirements.txt
```

---

## 📄 Licencia

Distribuido bajo la licencia [Apache 2.0](LICENSE).
