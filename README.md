# NLP Sarcasm Detection using BERT  
**Understanding Sarcasm in Political Discourse using NLP and Transformer-based Models**  

## 📌 Overview  
This repository contains the implementation of a **BERT-based sarcasm detection model** for analyzing political discourse on the **Ekşi Sözlük** platform. The project explores how sarcasm is used as a critique tool in online political discussions, particularly focusing on **Recep Tayyip Erdoğan** and **Kemal Kılıçdaroğlu**.

## 🚀 Key Features  
✅ **BERT-based Sarcasm Detection:** Fine-tuning **Bidirectional Encoder Representations from Transformers (BERT)** to identify sarcastic comments.  
✅ **Political Sentiment Analysis:** Analyzing sarcasm trends in online discussions related to Türkiye’s political landscape.  
✅ **Data Preprocessing & Annotation:** Cleaning, normalizing, and labeling data for sarcasm classification.  
✅ **Model Training & Performance Evaluation:** Evaluating BERT’s accuracy and effectiveness compared to other NLP models.  


---

## 📊 Dataset & Preprocessing  
### 📌 **Dataset Information**  
- The dataset is sourced from **Ekşi Sözlük**, a widely used online discussion platform in Türkiye.  
- It focuses on discussions about **Recep Tayyip Erdoğan** and **Kemal Kılıçdaroğlu**, covering **153,882 entries**.  
- The final **filtered dataset** consists of **107,432 entries**, ensuring high-quality text data for sarcasm detection&#8203;:contentReference[oaicite:0]{index=0}.  

### 🔄 **Preprocessing Steps**  
✔ **Removing biased authors:** Eliminated **30,525 entries** from prolific users to ensure balanced data.  
✔ **Filtering URLs and references:** Removed **4,066 reference-only entries** and **376 URL-only entries**.  
✔ **Length normalization:** Excluded entries shorter than **38 characters** or longer than **1,243 characters** to optimize performance.  
✔ **Tokenization & Normalization:** Applied **WordPiece Tokenization** and **BERT-compatible preprocessing**.  

---

## 🏗️ Methodology  
The sarcasm detection task is formulated as a **binary classification problem**:  
- **𝑆 = {𝑠1, 𝑠2, . . . , 𝑠𝑙} → 𝑌 = {0,1}** where  
  - `0 = Non-Sarcastic`
  - `1 = Sarcastic`  
- **Fine-tuning BERT:** The model learns sarcasm-specific **linguistic patterns**, identifying irony and contradictions.  
- **Hybrid Enhancements:** Used **Graph Convolutional Networks (GCNs)** and **Attention Mechanisms** to improve sarcasm context understanding&#8203;:contentReference[oaicite:1]{index=1}.  

---

## 📈 Results & Performance  

| Number of Entries | Annotated Sarcastic Entries | Precision | Recall | F1-Score | Accuracy |
|------------------|----------------------------|-----------|--------|----------|----------|
| 908             | 312                          | 0.77      | 0.53   | 0.63     | 0.79     |
| 1,038           | 405                          | 0.77      | 0.76   | 0.76     | 0.82     |
| **2,529**       | **864**                      | **0.79**  | **0.82**| **0.80** | **0.86** |

- **Sarcasm Trends by Political Figure**  
  - **28.1%** of Erdoğan-related entries were sarcastic.  
  - **9.2%** of Kılıçdaroğlu-related entries were sarcastic&#8203;:contentReference[oaicite:2]{index=2}.  
  - **Sarcasm peaks** during political and economic crises, indicating shifts in public sentiment.  

