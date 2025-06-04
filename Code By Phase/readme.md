# Project Phases

## Phase 1: Research Planning and Initial Study
- Conduct literature review

---

## Phase 2: Data Exploration and Preparation
1. Perform exploratory data analysis (EDA) to identify distribution patterns and anomalies  
2. Clean, standardize, and impute missing data  
3. Evaluate clustering methods (KMeans, Agglomerative, DBSCAN) through outlier detection and performance comparison  

---

## Phase 3: Data Derivation
- Use **gpt-40-mini** to extract side effects and effectiveness keywords from patient reviews  
- Steps involved:  
  1. Call OpenAI API Key  
  2. Initialize the model  
  3. Provide prompts for keyword extraction  

---

## Phase 4: Model Development and Evaluation
1. Apply sentiment-based filtering to reduce computational complexity  
2. Tokenize and vectorize text using TF-IDF  
3. Perform dimensionality reduction to retain 95% variance  
4. Tune DBSCAN parameters (epsilon, min samples)  
5. Achieve good clustering quality, but note inconsistencies within clusters  

**Planned Improvement with v2-ada model:**  
- Leverages semantic understanding to improve cluster consistency compared to TF-IDF  
- Still limited by information loss when pooling diverse side effects and effectiveness into fixed-size embeddings, affecting clustering accuracy  

---

## Additional: Data Visualization
- Visualize and explore cluster characteristics  

---

## **Future Work:**  
To address the limitations of TF-IDF, future work can explore advanced text representation techniques such as **Bag of Words**, **Word2Vec**, **BERT embeddings**, or **topic modeling**. These methods can better capture semantic meaning and variations in reported side effects and effectiveness, potentially improving clustering consistency and overall interpretability.
