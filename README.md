# 🎨 DoodleDetect — Sketch Recognition with CLIP + SVM + FAISS

DoodleDetect is a fun and intelligent sketch recognition system powered by OpenAI’s CLIP, Principal Component Analysis (PCA), Support Vector Machine (SVM), and FAISS for fast similarity search. Designed with both performance and personality, it includes a full-featured GUI, educational utility, and a mascot named Pixie to welcome you into the world of doodle classification.

> ✨ Whether you're drawing a palm tree, a windmill, or something in between — DoodleDetect is here to guess it (almost) correctly!

---

## 🚀 Live Demo

[![Watch Demo Video](https://github.com/jesslyntrixie/doodledetect/blob/main/pixie_and_robosketch.png)](https://binusianorg-my.sharepoint.com/personal/stanley_teguh_binus_ac_id/_layouts/15/guestaccess.aspx?share=EWMTcBZrBGlIn5gyOcwaEsoBwzRBb5vA8Un61D4uDgzJXw&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=hPtliy)

> 📽️ Click to watch how it works — draw, detect, delight!

---

## ✏️ Features

* 🎨 Draw your own sketches in an intuitive GUI
* 🔍 Real-time classification powered by CLIP + SVM + FAISS
* ⚡ Ultra-fast similarity-based retrieval using FAISS
* 📂 Log predictions and revisit previous drawings
* 💾 Save and load sketches in PNG format
* 📖 Learn how it works in the About section
* 🧙‍♂️ Meet Pixie — your AI mascot and personal guide!

---

## ⚙️ How to Run the App (Windows)

1. **Download the `.zip` release from [Releases](https://github.com/jesslyntrixie//DoodleDetect/releases)**
2. **Extract the zip** completely (⚠️ Do NOT run it from inside the archive)
3. **Double-click `doodledetect.exe`**
4. **Wait patiently!** It may take 5–10 seconds to load. Don’t click multiple times.

---

## 🧠 How It Works

### Training Pipeline (Python)

* ✨ **CLIP (ViT-B/32)** — Extracts semantic sketch features
* 📉 **PCA** — Reduces high-dimensional CLIP features to 256
* 🧮 **SVM (RBF)** — Classifies sketches based on reduced features
* 🔁 **FAISS** — Provides fast retrieval of visually similar sketches

All components are serialized and integrated into the app using `joblib`.

### Datasets Used

* **TU-Berlin** — 20,000 sketches from 250 categories
* **Sketchy** — 75,000+ sketches across 125 object classes

---

## 📈 Performance

| Dataset   | Top-1 Accuracy | Top-5 Accuracy |
| --------- | -------------- | -------------- |
| Sketchy   | 62.5%          | 81.2%          |
| TU-Berlin | 77.2% ✅        | 98.4% 🔥       |

> That’s even **better than human average performance** for Top-5 prediction!

---

## 📚 Dependencies

* `torch`, `transformers` — CLIP feature extraction
* `scikit-learn` — PCA, SVM, scaling
* `faiss-cpu` — 💡 FAISS for fast similarity search
* `tkinter`, `Pillow` — GUI and image rendering
* `joblib`, `numpy`, `os`, `csv`, `datetime`

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you’d like to change or add.

---

## 🧑‍💻 Credits

Developed by 📚 students of **Bina Nusantara University**  
Powered by the open-source ML ecosystem 🌍  
Special thanks to OpenAI, FAISS, HuggingFace, and the Python community!

---

## ⭐️ Show Some Love

If you enjoyed using or learning from this project, give it a star ⭐ and share it with your friends. Let’s make AI and creativity best friends again!
