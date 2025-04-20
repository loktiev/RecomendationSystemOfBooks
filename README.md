# README.md for RecomendationSystemOfBooks

## 📚 RecomendationSystemOfBooks
A basic recommendation system using **precomputed LightFM embeddings** and **NMSLIB** for fast nearest-neighbor search. This project demonstrates hybrid collaborative filtering on a small dataset.

---

## ⚙️ Installation

1. Clone the repository:
```bash
git clone https://github.com/loktiev/RecomendationSystemOfBooks.git
cd RecomendationSystemOfBooks
```

2. Create the conda environment:
```bash
conda env create -f environment.yml
```

3. Activate it:
```bash
conda activate recsys
```

4. Install NMSLIB manually (precompiled):
```bash
pip install path\to\nmslib‑2.1.1‑cp310‑cp310‑win_amd64.whl
```
> Download precompiled wheels from: https://www.lfd.uci.edu/~gohlke/pythonlibs/

⚠️ LightFM is **not required** for running the app as it uses pre-trained embeddings stored in `item_embeddings.pkl`.

---

## ▶️ Usage

### Run Streamlit web app:
```bash
streamlit run app.py
```

### Run NMSLIB test script (optional):
```bash
python Ex2.py
```
You should see a message: `✅ LightFM and NMSLIB are working!`

---

## 📁 Project Structure
```
RecomendationSystemOfBooks/
├── app.py                  # Streamlit interface
├── Ex2.py                  # Optional test script for NMSLIB
├── environment.yml         # Conda environment definition
├── requirements.txt        # Optional pip-only fallback
├── item_embeddings.pkl     # Precomputed embeddings
└── README.md               # Project overview (this file)
```

---

## 🛠 Notes
- `lightfm` is not used in production. You can remove it unless retraining is needed.
- `nmslib` is required and must be installed manually on Windows from prebuilt wheels.
- If using Streamlit Cloud, add `nmslib` and other dependencies into `requirements.txt` accordingly.

---

## 💡 License
This project is licensed under the MIT License.
