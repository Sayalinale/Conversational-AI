# Conversational-AI
# Fine-Tuning SBERT for Clarifying Ambiguous Questions

This project fine-tunes a Sentence-BERT (SBERT) model to handle ambiguous user queries by generating appropriate clarifying questions, enhancing conversational AI and search systems.

## 💡 Objective

To enable AI systems to respond to vague or ambiguous user queries with clarifying follow-up questions, improving the user experience in conversational search applications.

---

## 📂 Dataset

- Source: JSON file with user queries and human-generated clarifying questions.
- Format: Query-clarification pairs.

---

## ⚙️ Methodology

1. **Data Preprocessing**  
   - Loaded JSON data.
   - Extracted valid query-clarification pairs.
   - Saved clean data to CSV.

2. **Model Fine-Tuning**  
   - Model: `all-MiniLM-L6-v2` (SBERT).  
   - Loss Function: `MultipleNegativesRankingLoss`.  
   - Trained for 4 epochs with a warmup phase.

3. **Evaluation**  
   - Tested with cosine similarity between query and clarification embeddings.
   - High similarity scores indicate successful fine-tuning.

---

## 📊 Results

The fine-tuned model demonstrated strong performance in matching ambiguous queries to their clarifying questions, showing its potential for real-world use in chatbots and search assistants.

---

## 🚀 Future Improvements

- Expand dataset.
- Support for multilingual queries.
- Real-time chatbot integration.

---

## 🧑‍💻 Author

- Sayali Nale
