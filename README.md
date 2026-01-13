# Clasificación e interpretabilidad de tumores cerebrales (CNNs pre-entrenadas)

Proyecto de **Computer Vision** para clasificar imágenes de tumores cerebrales usando **redes neuronales pre-entrenadas (transfer learning)** y analizar **qué regiones de la imagen aportan más a la predicción** mediante técnicas de interpretabilidad (CAM).

---

## Objetivo

1) Verificar la **clasificación correcta** por tipo de tumor cerebral (3 clases).  
2) Identificar **componentes/regiones relevantes** de la imagen que influyen en la decisión del modelo (explicabilidad).

---

## Modelos y técnicas utilizadas

- **CNNs pre-entrenadas (Torchvision):** ResNet18, VGG16, EfficientNet-B0, MobileNetV2, DenseNet201  
- **Clasificadores (sobre embeddings / comparación):** Logistic Regression, SVM, Random Forest, XGBoost  
- **Reducción/visualización:** PCA, t-SNE  
- **Clustering/Exploración:** Self-Organizing Maps (MiniSom)  
- **Interpretabilidad:** Score-CAM (pytorch-grad-cam)  
- **Métricas:** classification report (precision/recall/F1), matriz de confusión

---

## Archivos

- `proyecto.ipynb` — Notebook principal del proyecto.
- `Brain_Cancer/` — Carpeta del dataset (estructura por clases).

---
## link del conjunto de datos
https://drive.google.com/drive/folders/1b-yI2hAqoC4OenQizd6LD7BwCam0iEG4

---
## Dataset (estructura esperada)

Coloca el dataset en una carpeta llamada `Brain_Cancer` con esta estructura:

```text
Brain_Cancer/
  Glioma/
    img_001.jpg
    ...
  Meningioma/
    img_001.jpg
    ...
  Tumor/
    img_001.jpg
    ...
## link del conjunto de datos
https://drive.google.com/drive/folders/1b-yI2hAqoC4OenQizd6LD7BwCam0iEG4
