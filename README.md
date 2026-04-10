# Auto Tagging Support Tickets Using LLM

## Objective
The objective of this project is to automatically classify support tickets into relevant categories using Large Language Models (LLMs). The system predicts the top 3 most probable tags for each ticket.

---

## Dataset
A free-text support ticket dataset is used.  
The dataset contains user queries such as login issues, payment problems, and technical bugs.

Example:
- "I cannot log into my account"
- "Payment was deducted twice"
- "App crashes when opening settings"

---

## Methodology / Approach

### 1. Zero-Shot Learning
The model classifies tickets without prior training using predefined categories.

### 2. Few-Shot Learning
A few labeled examples are provided in the prompt to improve classification accuracy.

### 3. Model Used
- LLM-based classification (zero-shot & few-shot)
- Alternative implementation using Hugging Face transformer model

### 4. Multi-Class Prediction
The system predicts:
- Top 3 tags
- Ranked based on confidence scores

---

## Model Development
- Input: Support ticket text
- Output: Top 3 predicted tags
- Techniques:
  - Prompt Engineering
  - Zero-shot classification
  - Few-shot learning

---

## Evaluation
- Compared zero-shot vs few-shot results
- Few-shot approach showed improved accuracy and relevance
- Output includes confidence scores for ranking

---

## Sample Output

Ticket: App crashes when opening settings

Top Tags:
1. Technical Bug (0.90)  
2. Performance Issue (0.80)  
3. App Crash (0.75)

---

## Technologies Used
- Python
- Transformers (Hugging Face)
- Pandas
- NLP (Natural Language Processing)

---

## Key Results / Observations
- Zero-shot provides decent baseline results
- Few-shot significantly improves prediction accuracy
- LLMs are effective for text classification without heavy training
- Multi-label tagging helps better categorize tickets

---

## Skills Gained
- Prompt Engineering
- LLM-based Text Classification
- Zero-shot and Few-shot Learning
- Multi-class Prediction and Ranking

---

## Conclusion
This project demonstrates how LLMs can automate support ticket classification efficiently. Few-shot learning enhances performance, making the system more reliable for real-world applications.
