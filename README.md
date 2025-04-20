# README.md for RecomendationSystemOfBooks

## 📚 RecomendationSystemOfBooks
A basic recommendation system using LightFM and NMSLIB. This project demonstrates hybrid collaborative filtering on a small dataset.

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

4. Install LightFM and NMSLIB manually (precompiled):
```bash
pip install path\to\lightfm‑1.17‑cp310‑cp310‑win_amd64.whl
pip install path\to\nmslib‑2.1.1‑cp310‑cp310‑win_amd64.whl
```
> Download precompiled wheels from: https://www.lfd.uci.edu/~gohlke/pythonlibs/

---

## ▶️ Usage

### Run Streamlit web app:
```bash
streamlit run app.py
```

### Run LightFM + NMSLIB script:
```bash
python Ex2.py
```
You should see a message: `✅ LightFM and NMSLIB are working!`

---

## 📁 Project Structure
```
RecomendationSystemOfBooks/
├── app.py                  # Streamlit interface
├── Ex2.py                  # Test script for LightFM + NMSLIB
├── environment.yml         # Conda environment definition
├── requirements.txt        # Optional pip-only fallback
└── README.md               # Project overview (this file)
```

---

## 🛠 Notes
- `scipy` and `backports.zoneinfo` were removed due to known compatibility issues with Python 3.10 + Conda.
- LightFM and NMSLIB are C++ extensions — install them from prebuilt wheels.

---

## 💡 License
This project is licensed under the MIT License.
