## 🎧 Multimodal Song Skip Prediction (Album Art Edition)

This project is an extension of my previous **Song Skip Prediction** model and asks a new question:  
> If we add **album cover images** on top of listening metadata, can we better predict which songs I’ll skip?

Here, I combine my Spotify extended streaming history with **album art embeddings** from **OpenAI CLIP (ViT-B/32)** and train an **XGBoost** classifier on the fused feature set, interpreting the model with **SHAP**. The full workflow from data processing to model interpretation is contained in the main notebook.

---

### 🚀 Getting Started

To reproduce this analysis, clone the repository and install the required packages.

**Prerequisites**
- Python 3.x  
- Jupyter Notebook or JupyterLab  

---

### 🧩 Installation

**1. Clone the repository**

    git clone https://github.com/your-username/song-skip-prediction-2.git
    cd song-skip-prediction-2

**2. Create and activate a virtual environment**

    python3 -m venv venv
    source venv/bin/activate   # On Windows: venv\Scripts\activate

**3. Install dependencies**  
(Uses `git+https://github.com/openai/CLIP.git` inside `requirements.txt`.)

    pip install -r requirements.txt

---

### 💻 Usage

Launch the Jupyter Notebook to see the code and analysis:

    jupyter notebook main.ipynb
