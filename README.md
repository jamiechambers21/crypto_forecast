# 🚀 Crypto Millionaire: A Data Science Adventure   
*Will this LSTM model make me rich? Probably not. But hey, let's give it a shot!*  

## 📜 Overview  
This project is my attempt at using **Deep Learning** (specifically LSTMs) to predict cryptocurrency prices. Exploring time series forecasting with historical crypto data, hoping to uncover patterns that *might* lead to financial glory (or at least a decent ML model).  

## 🏗️ Project Breakdown  

### 1️⃣ 📊 Data Collection  
- Fetched historical cryptocurrency data from **Binance API**.  
- Since Binance limits requests to 1000 rows, I cleverly (*or desperately*) looped over multiple API calls using `startTime` and `endTime` to get *all* available data.  

### 2️⃣ 🧹 Data Preprocessing  
- Converted timestamps, selected relevant columns, and normalized prices.  
- Created sequences of historical prices to feed into an **LSTM model**.  

### 3️⃣ 🧠 Model Development  
- Built a **Long Short-Term Memory (LSTM)** neural network with:  
  - **L2 regularization** (so it doesn’t go crazy and overfit).  
  - **Dropout layers** (because, let's be honest, overfitting is a real mood).  
- Trained multiple models with different hyperparameters to find the best one.  

### 4️⃣ 🏆 Hyperparameter Optimization  
- Tested different numbers of **LSTM units** and **dropout rates**.  
- Tracked performance using **validation loss**.  
- Selected the **best performing model** automatically.  

### 5️⃣ 📈 Predictions & Results  
- Evaluated model performance using **Mean Squared Error (MSE)**.  
- Plotted results to see if the model was predicting prices accurately or just hallucinating.  

---

## 💻 How to Run It  
```bash
# Clone the repo
git clone https://github.com/yourusername/crypto-millionaire.git
cd crypto-millionaire

# Install dependencies
pip install -r requirements.txt

# Run the data fetcher
python fetch_crypto_data.py

# Train the model
python train_model.py

# Make predictions
python predict.py
```
---

## 🔥 Will This Make Me a Millionaire?  
**Short answer:** Probably not.  
**Long answer:** Machine learning can find patterns, but **crypto markets are chaotic**. However, this project showcases valuable **time series forecasting skills** that are highly relevant in the **Data Science & AI industry**!  

---

## 📌 What I Learned  
✅ How to work with **real-world financial APIs** (Binance).  
✅ The importance of **data preprocessing** in time series forecasting.  
✅ How to build and fine-tune an **LSTM model** for predictions.  
✅ That predicting the future is **hard**.  

---

## 📢 Contributions & Feedback  
Want to improve the model or test new features? Feel free to **fork**, **star**, or open a **pull request**! Also, if you *do* become a millionaire using this, don’t forget to send me a **thank you tweet**. 😉  
