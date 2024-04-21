# ArtistIdentification
Este proyecto tiene como objetivo desarrollar un modelo de aprendizaje automático para identificar y clasificar estilos artísticos en ilustraciones. El enfoque principal es identificar el estilo particular de un artista (**@avogado6**) a través de ilustraciones donde haya personas.

## Información del Alumno
- **Nombre:** Ana Karen López Baltazar
- **Matrícula:** A01707750

## Conjunto de datos
### Origen del Conjunto de Datos
El conjunto de datos utilizado en este proyecto proviene de tres fuentes principales:

1. **@avogado6**: Ilustraciones del artista cuyo estilo se busca identificar. Imágenes recuperadas de su [página principal](https://www.avogado6.com/).
2. **@FutarinoTaiyou**: Ilustraciones de otro artista con un estilo similar. Imágenes recuperadas de su cuenta de [Twitter X](https://twitter.com/futarinotaiyou?lang=es).
3. **Kaggle Dataset**: Un conjunto de imágenes adicional obtenido de un dataset en Kaggle ([Pixiv Top Daily Illustration 2020](https://www.kaggle.com/datasets/stevenevan99/pixiv-top-daily-illustration-2020)) para complementar el conjunto de imágenes.

### Selección de Imágenes
Las imágenes seleccionadas para este proyecto se centran en ilustraciones de personas realizadas por el artista principal. Se han incluido imágenes que representan diferentes ángulos y perspectivas de las personas, incluyendo vistas de frente, de lado y parcialmente ocultas.

### División del Conjunto de Datos
El conjunto de datos se dividió en conjuntos de entrenamiento y prueba de manera aleatoria. Se asignó el 80% de las imágenes para el conjunto de entrenamiento y el 20% restante para el conjunto de prueba, asegurando una distribución equitativa de las imágenes entre ambos conjuntos.

- Conjunto de Entrenamiento: 520 imágenes
- Conjunto de Prueba: 130 imágenes
  
Para acceder al conjunto de datos completo utilizado en este proyecto, puedes visitar la siguiente liga de [Drive](https://drive.google.com/drive/folders/1CXb4dSFhRqj9K56XZ_WWbyvf4POauS17?usp=sharing).

### Preprocesamiento de Imágenes
Antes de alimentar los datos de imágenes al modelo de red neuronal, es esencial realizar un preprocesamiento adecuado para garantizar un mejor rendimiento de entrenamiento y generalización del modelo. En este proceso, las imágenes se redimensionaron a un tamaño uniforme de 256x256 píxeles y los valores de píxeles se escalonaron al rango [0, 1] dividiendo cada valor de píxel por 255.0. Además, se aplicaron técnicas de aumento de datos al conjunto de entrenamiento para incrementar artificialmente el tamaño del conjunto de datos y mejorar la capacidad del modelo para generalizar a datos no vistos. 
