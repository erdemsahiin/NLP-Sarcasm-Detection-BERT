# NLP Sarcasm Detection using BERT  
**Understanding Sarcasm in Political Discourse using NLP and Transformer-based Models**  

## 📌 Overview  
This repository contains the implementation of a **BERT-based sarcasm detection model** for analyzing political discourse on the **Ekşi Sözlük** platform. The project explores how sarcasm is used as a critique tool in online political discussions, particularly focusing on comparative analysis between **Recep Tayyip Erdoğan** and **Kemal Kılıçdaroğlu**.



## 🚀 Key Features  
✅ **BERT-based Sarcasm Detection:** Fine-tuning **Bidirectional Encoder Representations from Transformers (BERT)** to identify sarcastic comments.  
✅ **Political Sentiment Analysis:** Analyzing sarcasm trends in online discussions related to Türkiye’s political landscape.  
✅ **Data Preprocessing & Annotation:** Cleaning, normalizing, and labeling data for sarcasm classification.  
✅ **Model Training & Performance Evaluation:** Evaluating BERT’s accuracy and effectiveness compared to other NLP models.  



## 📊 Dataset & Preprocessing  
### 📌 **Dataset Information**  
- The dataset is sourced from **Ekşi Sözlük**, focusing on discussions about **Recep Tayyip Erdoğan** and **Kemal Kılıçdaroğlu**.  
- It contains **153,882** raw entries, which were **preprocessed and filtered down to 107,432 high-quality entries**.  
- **Irrelevant data (URLs, repetitive authors, references)** were removed to improve model accuracy.

### 🔄 **Preprocessing Steps**  
✔ **Removing biased authors:** Eliminated **30,525 entries** from prolific users.  
✔ **Filtering URLs and references:** Removed **4,066 reference-only entries** and **376 URL-only entries**.  
✔ **Length normalization:** Kept entries between **38–1,243 characters**.  
✔ **Tokenization & Normalization:** Applied **WordPiece Tokenization** and **BERT-compatible text processing**.



## 🏗️ Methodology  
- **Sarcasm detection is formulated as a binary classification task**:
  - `0 = Non-Sarcastic`
  - `1 = Sarcastic`
- **Fine-tuning BERT:** The model learns sarcasm-specific **linguistic patterns**, identifying irony and contradictions.



## 📈 Results 

### **Model Performance Metrics** 
| Number of Entries | Annotated Sarcastic Entries | Precision | Recall | F1-Score | Accuracy |
|------------------|----------------------------|-----------|--------|----------|----------|
| 908             | 312                          | 0.77      | 0.53   | 0.63     | 0.79     |
| 1,038           | 405                          | 0.77      | 0.76   | 0.76     | 0.82     |
| **2,529**       | **864**                      | **0.79**  | **0.82**| **0.80** | **0.86** |

### **Sarcasm Trends by Political Figure**  
| Figure              | Total Entries | Sarcasm Rate |  
|---------------------|---------------|--------------|  
| **Recep Tayyip Erdoğan** | 57,319        | **28.1%**    |  
| **Kemal Kılıçdaroğlu**   | 50,113        | **9.2%**     |  


## 📢 Conclusion  

### **Political Trends in Sarcasm Usage**  
The model identified a **major disparity** in sarcasm usage between political figures:  

- **Erdoğan-related entries had significantly more sarcasm (28.1%) compared to Kılıçdaroğlu (9.2%)**.  
- This suggests that **sarcasm is frequently used as an indirect tool of political criticism**, particularly targeting those in power.  
- **Criticism of opposition figures is lower**, indicating that sarcasm is a reaction to governance rather than opposition politics.

### **Why Is Sarcasm More Common for Erdoğan?**  
📌 **Heightened Political Criticism:**  
   - Erdoğan’s **central role in governance for over two decades** has made him a **prime target for public scrutiny**.  
   - Sarcasm allows for **indirect criticism**, especially in environments where **direct dissent is risky**.

📌 **Sarcasm Peaks During Political and Economic Crises:**  
   - **2018 Constitutional Reforms:** Led to increased sarcasm as executive powers expanded.  
   - **2019 Economic Crisis:** High inflation and government policies sparked sarcastic critiques like *"Erdoğan’s economic miracles"*.  
   - **2023 Elections:** Sarcasm peaked as Erdoğan won another term despite growing public discontent.

📌 **Differences Between Erdoğan & Kılıçdaroğlu in Sarcasm Trends:**  
   - **For Erdoğan**, sarcasm is **continuous and long-term**, reflecting **sustained dissatisfaction with governance**.  
   - **For Kılıçdaroğlu**, sarcasm is **situational**, mainly spiking during **elections or specific controversies**.
