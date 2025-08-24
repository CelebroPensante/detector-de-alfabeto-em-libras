# 🤟 AI Libras (Brazilian Sign Language) Alphabet Interpreter

An AI-powered system that interprets the **Brazilian Sign Language (Libras) alphabet** using computer vision and machine learning.  
The application leverages **MediaPipe** for hand landmark detection and a **Random Forest classifier** to recognize letters in real time through a webcam.  

This project aims to contribute to **accessibility and inclusion**, providing a foundation that can be extended to full word and sentence recognition in the future.  

---

## 📌 Features
- 🔹 Real-time recognition of Libras alphabet letters via webcam  
- 🔹 Hand landmark detection powered by Google **MediaPipe**  
- 🔹 Machine learning classification with **Random Forest**  
- 🔹 Visual feedback: bounding box and predicted letter displayed on screen  

---

## 🛠️ Technologies Used
- **Python** – main programming language  
- **OpenCV** – image processing and webcam capture  
- **MediaPipe** – hand tracking and landmark detection  
- **scikit-learn** – machine learning model training (Random Forest)  
- **NumPy** – data handling and preprocessing  

---

## 📂 Project Structure
```

.
├── data/                # Training dataset (organized in folders by letter)
├── models/              # Saved ML model
├── training.py          # Train the Random Forest classifier
├── collect\_data.py      # Process images and generate training dataset
├── real\_time.py         # Real-time prediction with webcam
├── requirements.txt     # Dependencies
└── README.md            # Project documentation

````

---

## 🚀 Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/usuario/repo.git
   cd repo
````

2. **Create a virtual environment (recommended)**

   ```bash
   python -m venv venv
   source venv/bin/activate   # Linux/Mac
   venv\Scripts\activate      # Windows
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

---

## ▶️ Usage

1. **Prepare dataset**
   Place images of hands performing Libras alphabet signs inside `./data/` with one folder per letter.

2. **Generate training data**

   ```bash
   python collect_data.py
   ```

3. **Train the model**

   ```bash
   python training.py
   ```

4. **Run real-time prediction**

   ```bash
   python real_time.py
   ```

---

## 📊 Results

* Achieved **high accuracy** in recognizing the Libras alphabet during testing
* Works in **real-time** with low latency
* Robust under different lighting conditions (but still room for improvement)

---

## ⚡ Challenges

* Building a consistent dataset with enough variety of hand positions and lighting conditions
* Maintaining real-time performance while processing landmarks and predictions

---

## 🌱 Future Improvements

* Expand dataset to support **words and full sentences** in Libras
* Optimize the model for **mobile devices**
* Add **voice output** for recognized letters/words
* Improve UI/UX for accessibility

---

## 📜 License

This project is released under the [MIT License](LICENSE).

---

## 👨‍💻 Author

Developed by **[Vitor G. J. de Carvalho](https://github.com/usuario)**

