# 🔮 Predicting Next Word

## Motivation
Autocomplete systems have become a staple in modern applications, making typing faster and smarter.  
This project builds a next-word prediction model using deep learning to mimic these features in a simple command-line interface.

---

## Project Goals
- Train an RNN/LSTM model to predict the **most likely next word** given an input phrase  
- Provide a script (`predict.py`) to get instant predictions  
- Offer a clean and modular codebase for experimentation and learning  

---

## Project Approach
- **Data preprocessing** → Tokenize text, build vocabulary, create input-output sequences  
- **Model architecture** → Train an LSTM-based language model in `model.py`  
- **Training script** → `train.py` handles training loop, checkpoint saving  
- **Prediction script** → `predict.py` performs tokenization and next-word inference  

---

## Example Usage
```bash
# Install dependencies
pip install -r requirements.txt

# Train model
python src/train.py --data data/sample_texts.txt --epochs 10

# Predict next word
python src/predict.py "The quick brown"
> Next word: fox
Technologies Used
Python

TensorFlow / Keras (for RNN/LSTM)

Numpy, Pandas for data handling

Project Outcome
A functioning next-word prediction model

Scripts for training and live inference

Modular design for easy extension (e.g., beam search, web interface)

Run Locally
Clone the repository

bash
Copy code
git clone https://github.com/your-username/Predicting-Next-Word.git
cd Predicting-Next-Word
Install dependencies

bash
Copy code
pip install -r requirements.txt
