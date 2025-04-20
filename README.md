# README.md for RecomendationSystemOfBooks

## 📚 RecomendationSystemOfBooks
A basic recommendation system using **precomputed embeddings** and **scikit-learn** for fast nearest-neighbor search. This project demonstrates hybrid collaborative filtering on a small dataset.

---

## ⚙️ Installation

1. Clone the repository:
```bash
git clone https://github.com/loktiev/RecomendationSystemOfBooks.git
cd RecomendationSystemOfBooks
```

2. (Recommended) Create and activate a virtual environment:
```bash
conda create -n recsys python=3.10 -y
conda activate recsys
```

3. Install required dependencies:
```bash
pip install -r requirements.txt
```

---

## ▶️ Usage

### Run Streamlit web app:
```bash
streamlit run app.py
```

---

## 📁 Project Structure
```
RecomendationSystemOfBooks/
├── app.py                  # Streamlit interface
├── environment.yml         # Optional Conda environment definition
├── requirements.txt        # Pip dependencies
├── item_embeddings.pkl     # Precomputed embeddings
├── data/                   # Ratings and books CSV files
└── README.md               # Project overview (this file)
```

---

## 🛠 Notes
- `lightfm` and `nmslib` are **no longer required** for app deployment.
- The application uses precomputed item embeddings (`item_embeddings.pkl`) and Scikit-learn's `NearestNeighbors` for similarity search.
- You can deploy this app on Streamlit Cloud with a clean and simple requirements setup.

---

## 💡 License
This project is licensed under the MIT License.
