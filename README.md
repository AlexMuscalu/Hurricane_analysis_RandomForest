# 🌪 Hurricane Classification – Machine Learning Project

Proiect realizat în cadrul cursurilor de **Tehnici de Colectare și Manipulare a Datelor** și **Data Mining și Învățare Automată**, parte a programului de masterat **Data Science și Inteligență Artificială**.

Scopul acestui proiect este construirea unui model de învățare automată care să poată **prezice dacă o furtună tropicală va deveni uragan**, pe baza unor variabile precum viteza vântului, presiunea atmosferică, locația geografică și momentul înregistrării.

---

## 📁 Structura fișierelor
- `hurricane_classification.ipynb` – notebook-ul complet cu cod, explicații și rezultate
- `storms.csv` – setul de date cu furtuni tropicale (sursă: Kaggle/NOAA)
- `README.md` – acest fișier

---

## 🧠 Obiective
- Prelucrarea și curățarea datelor reale
- Vizualizarea relațiilor între variabile meteorologice
- Construirea unui model de clasificare binară (Random Forest)
- Evaluarea performanței modelului pe un set de testare
- Aplicabilitate în sisteme de avertizare timpurie

---

## 🔍 Datele utilizate

Setul de date conține peste **19.000 de înregistrări** ale furtunilor din Atlantic, colectate la fiecare 6 ore. Fiecare observație include:
- Momentul înregistrării: `year`, `month`, `day`, `hour`
- Locația: `lat`, `long`
- Condiții: `wind`, `pressure`, `storm force diameter`
- Etichetă țintă: `is_hurricane` (1 = uragan, 0 = furtună)

---

## 📊 Explorare și analiză

- Corelații relevante:
  - `wind` are o corelație pozitivă puternică cu `is_hurricane` (0.82)
  - `pressure` are o corelație negativă puternică (−0.76)
- Distribuția dezechilibrată a claselor (majoritatea observațiilor nu sunt uragane)
- Vizualizări realizate cu `seaborn` și `matplotlib`

---

## 🤖 Model de clasificare

- Algoritm: `RandomForestClassifier`
- Împărțire date: 80% antrenare, 20% testare
- Metrici de evaluare:
  - **Accuracy**: 100%
  - **Recall (uragane)**: 99%
  - **F1-score**: 0.99
  - **AUC (ROC Curve)**: 1.00

🔍 Modelul a identificat aproape toate uraganele reale, cu doar 4 greșeli în total (din 1911 cazuri).

---

## ✅ Concluzii

Modelul Random Forest oferă o clasificare de înaltă acuratețe pentru furtuni, folosind doar caracteristici fizice simple. Proiectul demonstrează cum poate fi utilizat un model ML pentru **predicția fenomenelor meteorologice extreme**, având potențial de utilizare practică în:
- Sisteme de avertizare timpurie
- Analiză de risc meteorologic
- Predicții automate pentru aplicații meteo

---

## 🚀 Ce am învățat

✔️ Cum să curăț și structurez un set de date real  
✔️ Cum să identific variabile predictive prin analiză statistică  
✔️ Cum să antrenez un model ML și să-l evaluez profesionist  
✔️ Cum să structurez un proiect complet pentru GitHub/portofoliu

---

## ✍️ Autor

**Alex Muscalu**  
Masterand în Data Science și AI  
Universitatea Titu Maiorescu  
📍 România  
🎸 Pasionat de muzică, automatizare și inteligență artificială

---

## 📎 Licență

Distribuit sub licență MIT.
