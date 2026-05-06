# TOPSIS-Based Selection of Best Pretrained Model for Text Generation

## 📌 Objective

The objective of this project is to apply the **TOPSIS (Technique for Order Preference by Similarity to Ideal Solution)** method to identify the most suitable pretrained model for **text generation**, based on multiple evaluation criteria.

---

## 🤖 Models Considered

The following pretrained language models were evaluated:

* GPT-2
* DistilGPT-2
* GPT-Neo
* DialoGPT
* Bloom

---

## 📊 Evaluation Criteria

The models were compared using the following criteria:

* **Quality** → Higher is better
* **Inference Time** → Lower is better
* **Model Size** → Lower is better

---

## ⚙️ Methodology

The TOPSIS method was implemented using the following steps:

1. Constructed a **decision matrix** using model performance data
2. Applied **vector normalization** to standardize values
3. Assigned weights to each criterion:

   * Quality → 0.5
   * Inference Time → 0.3
   * Model Size → 0.2
4. Computed the **weighted normalized decision matrix**
5. Determined:

   * Ideal Best Solution
   * Ideal Worst Solution
6. Calculated the **Euclidean distance** of each model from:

   * Ideal Best
   * Ideal Worst
7. Computed the **TOPSIS score** and ranked the models

---

## 📈 Results

* Each model was assigned a TOPSIS score based on its relative performance
* Models were ranked accordingly
* The model with the **highest TOPSIS score** is considered the best choice

### 🔹 Score Table

![TOPSIS Scores](https://github.com/user-attachments/assets/b55058d2-fc11-4a02-b6c0-f7321829dd68)

### 🔹 Ranking Visualization

![Ranking Plot](https://github.com/user-attachments/assets/829c8638-6316-41b0-99d3-81bccb8ef5b6)

---

## 🔍 Observations

* Models with higher **text quality** tend to rank better despite larger size
* Trade-offs between **speed and performance** significantly affect ranking
* Weight selection plays a critical role in determining final outcomes

---

## 🚀 Conclusion

This project demonstrates how **multi-criteria decision-making techniques like TOPSIS** can be effectively used to select the most suitable pretrained model for real-world tasks such as text generation.

---

## 🛠️ Future Improvements

* Include additional metrics (e.g., perplexity, memory usage)
* Perform evaluation on larger benchmark datasets
* Compare with other decision-making methods (e.g., AHP, VIKOR)
* Automate evaluation pipeline for dynamic model comparison
