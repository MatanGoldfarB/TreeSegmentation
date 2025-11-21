# Tree Segmentation  
A YOLOv8 segmentation model trained on a custom dataset of approximately 2,400 annotated images of tree canopies and groves. This project demonstrates my ability to collect and label data, configure modern object segmentation models, and train them to accurately segment tree structures from aerial imagery.  

## 🎥 Project Demo  
 <img width="640" height="480" alt="TreeSeg3" src="https://github.com/user-attachments/assets/3b664503-a94c-4c7f-978a-c4856ea792b5" />
<img width="640" height="480" alt="TreeSeg2" src="https://github.com/user-attachments/assets/ef8310d4-4157-45b5-b118-dafef229511f" />
<img width="640" height="480" alt="TreeSeg1" src="https://github.com/user-attachments/assets/a82b6353-5d20-4bf9-84c3-a5328454ad84" />

*(If the video preview doesn’t load, click the link to view the .mov directly.)*  

## 📦 Dataset  
- **Source:** Custom dataset hosted on Roboflow (tree-grove-seg).  
- **Size:** ~2,400 images with pixel-level annotations.  
- **Classes:** 2 classes – `grove` and `tree`.  
- **Structure:** Standard YOLO segmentation format with separate `train/images` and `valid/images` directories (see `config.yaml`).  

## 🚀 Model & Training  
- **Model:** YOLOv8 Segmentation (Ultralytics).  
- Training performed via the notebook `train.ipynb`.  
- Configuration defined in `config.yaml` (dataset paths, class names, number of classes).  
- Uses the Ultralytics Python package to run training loops and evaluate metrics.  

## 🧰 How to Run  
1. **Clone the repository:**  
   ```bash  
   git clone https://github.com/MatanGoldfarB/TreeSegmentation  
   cd TreeSegmentation  
   ```  
2. **Install dependencies:**  
   ```bash  
   pip install ultralytics roboflow  
   ```  
3. **Download the dataset:**  
   - Create a Roboflow account and download the `tree-grove-seg` dataset in YOLOv8 segmentation format.  
   - Place the dataset under a `data/` directory and update the `path`, `train`, and `val` fields in `config.yaml` if necessary.  
4. **Run training:**  
   - Open `train.ipynb` in Jupyter Notebook or VS Code.  
   - Adjust file paths as needed (see comments in the notebook).  
   - Execute the cells to train the model.  

## 🗂 Repository Structure  
```
TreeSegmentation/
├── runs/           # YOLO training runs (weights, metrics, etc.)  
├── config.yaml     # Dataset and class configuration  
├── train.ipynb     # Jupyter notebook for training  
└── README.md       # Project documentation  
```  

## 📍 What This Project Demonstrates  
This project highlights my experience in:  
- Data collection and annotation for computer vision tasks.  
- Configuring and training a state-of-the-art segmentation model (YOLOv8).  
- Working with Python-based ML frameworks and Jupyter notebooks.  
- Documenting and sharing experiments for reproducibility.  

## 🛠 Future Work  
- Evaluate segmentation accuracy on larger and more diverse datasets.  
- Incorporate model quantization or pruning for deployment on edge devices.  
- Fine-tune hyperparameters and use augmentation techniques to improve performance.  

## 💌 Contact  
For more information or collaborations, feel free to reach out.
