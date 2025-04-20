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

To run the Streamlit web app locally:
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
├── item_embeddings.pkl     # Precomputed item embeddings
├── data/                   # Ratings and books CSV files
└── README.md               # Project overview
```

---

## 🛠 Notes
- ✅ `lightfm` and `nmslib` are **no longer required** for app deployment.
- ✅ Uses `scikit-learn`'s `NearestNeighbors` with precomputed vectors (`item_embeddings.pkl`).
- ✅ Compatible with deployment on **Streamlit Cloud** using a minimal `requirements.txt`.

---

## 💡 License
This project is licensed under the MIT License.
