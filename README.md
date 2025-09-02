# Clasificación de Emociones en Tweets (EmoEvent)

## ⚙️ Modelos Implementados
1. **TF-IDF + Regresión Logística**  
   - Modelo baseline con representaciones TF-IDF.  
   - Ventaja: rápido y sencillo de entrenar.  
   - Limitación: tiende a predecir clases dominantes.

2. **BiLSTM**  
   - Modelo secuencial con embeddings entrenados.  
   - Potencial para capturar dependencias contextuales.  
   - Limitación: requiere más datos/ajuste para superar al baseline.

3. **Embeddings + SVM**  
   - Modelo basado en representaciones semánticas preentrenadas con un clasificador SVM.  
   - Resultó ser el más robusto y equilibrado.  

---

## 📊 Resultados Globales

| Modelo           | Accuracy | Macro-F1 | Weighted-F1 |
|------------------|----------|----------|-------------|
| **Embeddings+SVM** | **0.587** | **0.330** | **0.548** |
| TFIDF+LR         | 0.546    | 0.281    | 0.498       |
| BiLSTM           | 0.509    | 0.254    | 0.470       |