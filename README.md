# 🎨 WGAN-GP CIFAR-10 Explorer

An end-to-end Generative AI project featuring a **Wasserstein GAN with Gradient Penalty (WGAN-GP)** trained on the CIFAR-10 dataset. This repository includes a high-performance **FastAPI** backend and an interactive **Streamlit** frontend.

---

## 🚀 Overview

This project demonstrates the full lifecycle of a Deep Learning application:
1.  **Training:** Developed a WGAN-GP in TensorFlow/Keras on Kaggle (GPU-accelerated).
2.  **Stability:** Used Gradient Penalty to ensure stable convergence and high-quality image generation.
3.  **Deployment:** Created a REST API to serve model inferences locally.
4.  **UI/UX:** Built a "Slot Machine" dashboard for users to interact with the AI hallucinations.

---

## 🛠️ Tech Stack

* **Model:** TensorFlow / Keras 3 (WGAN-GP)
* **Backend:** FastAPI (Uvicorn)
* **Frontend:** Streamlit
* **Data:** CIFAR-10 Dataset
* **Processing:** NumPy, Pillow (PIL), OpenCV

---

## 📂 Project Structure

```text
WGAN_Project/
├── backend/
│   ├── main.py            # FastAPI Inference Engine
│   └── generator.keras    # Trained WGAN Model Weights
├── frontend/
│   └── app.py             # Streamlit Interactive Dashboard
└── README.md              # Documentation
⚙️ Installation & Setup
1. Clone the repository
Bash
git clone [https://github.com/YOUR_USERNAME/WGAN-CIFAR10.git](https://github.com/YOUR_USERNAME/WGAN-CIFAR10.git)
cd WGAN-CIFAR10
2. Install Dependencies
Bash
pip install fastapi uvicorn tensorflow streamlit pillow requests numpy
3. Add the Model
Place your generator.keras file inside the backend/ folder.

🏃 How to Run
You will need two terminal windows open:

Step 1: Start the Backend

Bash
cd backend
python main.py
Step 2: Start the Frontend

Bash
cd frontend
streamlit run app.py
🎰 Key Features
1. AI Slot Machine
A gamified interface where users "Spin the GAN." It features a custom animation that simulates "shuffling" before displaying three freshly generated 32x32 images.

2. Real vs Generated Comparison
Allows users to benchmark the model's performance by comparing a random real image from the CIFAR-10 dataset side-by-side with an AI-generated image.

🧠 Model Insights
The Wasserstein GAN with Gradient Penalty was chosen over standard GANs to prevent Mode Collapse and Vanishing Gradients. By using the Earth Mover's Distance, the model provides a reliable loss metric that correlates with image quality.

📄 License
This project is open-source and available under the MIT License.


### Next Step for GitHub:
Since you are uploading to GitHub, would you like me to help you write a **`.gitignore
