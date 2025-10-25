# 🧠 Análisis de Importancia de Palabras con TF-IDF y spaCy

Este proyecto calcula la **importancia global de las palabras** en un conjunto de textos utilizando **TF-IDF (Term Frequency – Inverse Document Frequency)**, y elimina las *stopwords* (palabras vacías) usando **spaCy** para obtener resultados más limpios y relevantes.

---

## 🚀 Descripción del proceso

1. **Vectorización del texto con TF-IDF**  
   Se utiliza `TfidfVectorizer` de *scikit-learn* para convertir una lista de documentos en una matriz TF-IDF.  
   Cada valor representa la importancia de una palabra dentro de un documento.

2. **Cálculo del TF-IDF global**  
   Se suman los pesos TF-IDF por palabra a través de todos los documentos, para obtener su importancia total en el corpus.

3. **Eliminación de stopwords con spaCy**  
   Se cargan las stopwords del modelo `es_core_news_sm` y se filtran las palabras irrelevantes (como “el”, “de”, “y”, “la”, etc.).

4. **Visualización de las palabras más importantes**  
   Se grafica un diagrama de barras con las palabras más relevantes (sin stopwords) y su valor TF-IDF total.

---

