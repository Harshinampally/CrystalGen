🧊 CrystalGen: AI-Powered Crystal Structure Generator 

CrystalGen is an AI-powered web application built with Flask that generates and visualizes crystal structures using a Conditional Variational Autoencoder (CVAE).
It allows users to configure parameters such as space group, composition, and temperature, and instantly generate realistic 3D crystal lattices.

🌐 Overview

CrystalGen integrates:

🧠 Deep Learning (CVAE) for structure generation

🔬 Pymatgen for CIF parsing and structure validation

🧱 Torch Geometric (PyG) for crystal graph representation

🌍 Flask Backend + HTML/JS Frontend for seamless web experience

🎨 3D visualization (Three.js / Plotly / Py3Dmol) for viewing atomic structures



project structure 


<img width="266" height="717" alt="image" src="https://github.com/user-attachments/assets/c61a8c5f-e502-4925-bd18-b0011ce574d3" />





---

## ⚙️ Installation Guide

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/<your-username>/CrystalGen.git
cd CrystalGen


python -m venv venv
venv\Scripts\activate      # Windows
# or
source venv/bin/activate   # Mac/Linux


pip install -r requirements.txt
python app.py



🧠 Model Description

CrystalGen uses a Conditional Variational Autoencoder (CVAE) to model complex crystal formation patterns.
The encoder converts input graphs into latent space representations, the diffusion layer introduces structural variations, and the decoder reconstructs valid 3D structures.

Model Architecture:

Encoder: Compresses input crystal graphs into a latent vector

Latent Diffusion: Adds controlled stochasticity for realistic diversity

Decoder: Generates 3D atomic coordinates and lattice parameters

Output: CIF structure + interactive visualization
