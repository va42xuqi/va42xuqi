# 🧠 ML Prototype Template

Ein minimales, sauberes Projekt-Template für ML-/DL-Experimente mit PyTorch und Python.

## 📁 Projektstruktur

```
ml-project/
├── data/                 # Rohdaten oder vorbereitete Datensätze
├── notebooks/            # Jupyter/Colab-Notebooks
├── src/                  # Python-Module (Training, Modelle, Evaluation)
│   ├── models.py
│   ├── train.py
│   ├── evaluate.py
│   └── utils.py
├── outputs/              # Ergebnisse, Plots, Logs
├── README.md
├── requirements.txt
└── .gitignore
```

## 🚀 Schnellstart

```bash
# Umgebung aufsetzen (z.B. mit venv oder conda)
pip install -r requirements.txt

# Training starten
python src/train.py --config configs/default.yaml
```

## ⚙️ Abhängigkeiten

```txt
pytorch
numpy
pandas
matplotlib
scikit-learn
```

> Optional: wandb, hydra, tqdm

## 🧪 Beispiel: Trainingseintrag (train.py)

```python
from models import MyModel
from utils import load_data

model = MyModel()
data = load_data()

# Trainieren
def train(model, data):
    for epoch in range(10):
        loss = model.fit(data)
        print(f"Epoch {epoch}, Loss: {loss:.4f}")
```

## 📝 Lizenz

MIT License – frei nutzbar und erweiterbar

---
