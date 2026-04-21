# Masked Face Recognition

## ⚠️ Disclaimer / Aviso

**English**

This repository contains the code developed for my undergraduate thesis, completed approximately five years ago during the COVID-19 pandemic. The project explores face recognition techniques adapted to masked faces.

Please note that this code reflects my knowledge and development practices at that time. It may not follow current best practices, libraries, or standards, and it is not actively maintained. The repository is provided for educational, archival, and reference purposes only.

Additionally, this project was developed in an academic context using limited datasets and simulated masks. It is not intended for production use or real-world deployment, particularly in sensitive applications involving biometric identification.

---

**Español**

Este repositorio contiene el código desarrollado para mi Trabajo de Fin de Grado, realizado hace aproximadamente cinco años durante la pandemia de COVID-19. El proyecto explora técnicas de reconocimiento facial adaptadas a rostros con mascarilla.

Debe tenerse en cuenta que este código refleja los conocimientos y prácticas de desarrollo de ese momento. Puede no seguir las mejores prácticas, librerías o estándares actuales, y no se encuentra mantenido activamente. Se proporciona únicamente con fines educativos, de referencia y archivo.

Además, este proyecto fue desarrollado en un contexto académico utilizando datasets limitados y mascarillas simuladas. No está destinado a uso en producción ni a su despliegue en entornos reales, especialmente en aplicaciones sensibles relacionadas con la identificación biométrica.

## README.md


# Masked Face Recognition using CNNs as feature extractor, PCA for dimensionality reduction and Machine Learning classifiers


Due to the current world situation, the COVID-19 crisis, the use of face masks has become widespread. When attempting to apply the vast majority of existing face recognition techniques on a masked or partially covered face, a significant decrease in performance is observed. This is due to the lack of information and features produced by the occlusion of facial features.

The main goal of this project is to implement a system capable of applying face recognition on images containing people wearing masks. 
For this purpose, the AT & T Laboratories Cambridge ORL dataset has been used. This dataset contains 400 images of 40 people. 
Wear-Mask-To-Face has been adapted to our workspace (Colaboratory) to place a mask on each image of the dataset. 

More information about the original implementation of Wear-Mask-To-Face: https://github.com/Amoswish/wear_mask_to_face

The implementation performs feature extraction using a CNN without the last classification layers, then we use PCA to reduce dimensionality, and finally a classifier is applied.
For this purpose, several pre-trained CNN models and classifiers have been used.
  
CNN models used:
* VGG16
* VGG19
* ResNet50
* ResNet101
* InceptionV3
    
Classifiers:
* MLP
* SVM (LinearSVC)
* Random Forest

Best perfomance models:
  1.  VGG16 + LinearSVC   (~ 94% Accuracy, 0.97 AUC)
  2.  VGG16 + MLP         (~ 93% Accuracy, 0.97 AUC)
  3.  VGG19 + LinearSVC   (~ 92% Accuracy, 0.96 AUC)

This repository contains the entire project developed in Google Colaboratory notebooks.

---

# Reconocimiento facial con uso de mascarilla empleando CNNs como extractor de características, PCA para reducción de dimensionalidad y clasificadores Machine Learning


Debido a la situación mundial actual, la crisis del COVID-19, se ha extendido el uso de mascarillas. Al intentar aplicar la gran mayoría de técnicas existentes de reconocimiento facial sobre una cara con mascarilla o parcialmente tapada, se observa una gran disminución de su rendimiento. Esto es debido a la falta de información y características producida por la oclusión de facciones.

El principal objetivo de este proyecto es implementar un sistema capaz de aplicar reconocimiento facial en imágenes que contienen personas haciendo uso de mascarilla. 
Para ello se ha empleado el dataset ORL de AT & T Laboratories Cambridge. Este dataset contiene 400 imagenes de 40 personas. 

Se ha adaptado Wear-Mask-To-Face a nuestro espacio de trabajo (Colaboratory) para colocar una mascarilla en cada imagen del dataset. 

Más información sobre la implementación original de Wear-Mask-To-Face: https://github.com/Amoswish/wear_mask_to_face

La implementación realiza la extracción de características mediante una CNN sin las últimas capas de clasificación, posteriormente empleamos PCA para reducir dimensionalidades, y por último se emplea un clasificador.
Para ello se han empleado varias redes CNN preentrenadas y clasificadores ML.
  
Redes CNN empleadas:
* VGG16
* VGG19
* ResNet50
* ResNet101
* InceptionV3

Clasificadores:
* MLP
* SVM (LinearSVC)
* Random Forest

Mejores modelos:

  1.  VGG16 + LinearSVC   (~ 94% Accuracy, 0.97 AUC)
  2.  VGG16 + MLP         (~ 93% Accuracy, 0.97 AUC)
  3.  VGG19 + LinearSVC   (~ 92% Accuracy, 0.96 AUC)


Este repositorio contiene los ficheros del proyecto desarrollado en cuadernos de Google Colaboratory.
