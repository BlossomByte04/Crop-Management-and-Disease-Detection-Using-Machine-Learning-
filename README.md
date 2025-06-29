
🌾 Crop Disease Detection & Management System
============================================

A deep learning-based plant disease classification and management tool using **ResNet-9** and **PyTorch**  
🔬 Built to aid **farmers** and **agriculture researchers** in early diagnosis and smart interventions.

------------------------------------------------------------
📌 Features
------------------------------------------------------------
✅ Detects 38 Plant Diseases across multiple crops  
✅ Powered by ResNet-9 with custom residual blocks  
✅ Data Augmentation Ready – Works on augmented datasets  
✅ GPU Accelerated – Supports CUDA for fast training  
✅ Visual Insights – Graphs and batch image previews included  
✅ Model Persistence – Trained model saved as `.pth` for reuse  
✅ Validation + Accuracy Visualization – Epoch-wise loss, accuracy, and learning rate graphs

------------------------------------------------------------
📂 Project Structure
------------------------------------------------------------
📁 Crop-Disease-Detector/  
│── README.txt ← Project documentation  
│── Plant_Disease_Detection.ipynb ← Full training + evaluation pipeline  
│── dataset/ ← Train, valid, test directories with images  
│── plant-disease-model.pth ← Trained model weights  
│── plant-disease-model-complete.pth ← Entire model saved  

------------------------------------------------------------
🔧 Installation & Setup
------------------------------------------------------------

1️⃣ Clone the Repository
------------------------
git clone https://github.com/BlossomByte04/Crop-Disease-Detection-Management-System.git
cd Crop-Disease-Detection-Management-System

2️⃣ Set Up Python Environment (Optional but Recommended)
---------------------------------------------------------
python -m venv venv
source venv/bin/activate      # Mac/Linux
venv\Scripts\activate       # Windows

3️⃣ Install Dependencies
-------------------------
pip install torch torchvision torchaudio matplotlib pandas pillow
pip install torchsummary

4️⃣ Run Jupyter Notebook
-------------------------
jupyter notebook Plant_Disease_Detection.ipynb

------------------------------------------------------------
🧠 Model Details
------------------------------------------------------------
- Architecture: ResNet-9 with custom residual connections  
- Base Class: ImageClassificationBase – handles training & validation  
- Loss Function: Cross Entropy  
- Optimizer: Adam / SGD with OneCycleLR scheduler  
- Performance Metrics: Validation accuracy, loss curves, LR decay  
- Model Save Paths: 
  - plant-disease-model.pth – weights only  
  - plant-disease-model-complete.pth – full model

------------------------------------------------------------
🖼️ Dataset Overview
------------------------------------------------------------
- Source: New Plant Diseases Dataset (Augmented)  
- 38 Classes of diseases from various crops  
- Uses ImageFolder from torchvision.datasets  

------------------------------------------------------------
📊 Example Outputs
------------------------------------------------------------
- Disease classification from test images  
- Validation accuracy/loss vs. epochs  
- Learning rate decay curve  

------------------------------------------------------------
🛠️ Tech Stack
------------------------------------------------------------
- Python 3.8+  
- PyTorch + torchvision  
- matplotlib, pandas, numpy  
- torchsummary, PIL  
- Google Colab / Jupyter Notebook  

------------------------------------------------------------
🔮 Future Enhancements
------------------------------------------------------------
- Mobile version with ONNX/TensorFlow Lite  
- Real-time inference via FastAPI/Streamlit  
- Disease Management Recommendations  
- Edge deployment with Raspberry Pi or Jetson Nano  

------------------------------------------------------------
🤝 Team Contributions
------------------------------------------------------------
Built as a team project to improve:
- Deep Learning and CNNs  
- Team collaboration & Git workflows  
- Data visualization & reporting  
- Model optimization & deployment  

------------------------------------------------------------
📬 Example Code Snippet
------------------------------------------------------------
from PIL import Image  
img = Image.open("test_leaf.jpg")  
predicted = predict_image(img_tensor, model)  
print("Predicted disease:", predicted)

------------------------------------------------------------
📎 References
------------------------------------------------------------
- Plant Village Dataset: https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset  
- ResNet Paper: https://arxiv.org/abs/1512.03385

------------------------------------------------------------
🌱 Supports SDG Goal 2: Zero Hunger
------------------------------------------------------------
