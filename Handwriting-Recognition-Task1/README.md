# Handwriting Recognition - Task 1
## Digit Recognition with CNN on MNIST Dataset

### 👥 Team Members
- **Member 1**: Chatti Mohamed Louay - Data Analysis & Preprocessing
- **Member 2**: Laouini Mohamed Amine - Model Architecture & Training  
- **Member 3**: Benyahya Yassine - Evaluation & Documentation

### 🎯 Project Objectives
Build a robust digit recognition system using MNIST dataset and compare CNN architectures with various improvements including dropout, batch normalization, and data augmentation.

### 📊 Results Summary
| Model | Test Accuracy | Test Loss | Parameters | Improvements |
|-------|---------------|-----------|------------|--------------|
| Baseline CNN | 99.10% | 0.0283 | ~1.2M | - |
| Improved CNN | 99.44% | 0.0684 | ~2.8M | Dropout, Data Augmentation, BatchNorm |

**Accuracy Improvement**: +0.34% (meaningful enhancement given high baseline performance)

### 🏗️ Methodology

#### Dataset
- **MNIST Dataset**: 70,000 grayscale images (60,000 training + 10,000 testing)
- **Image Dimensions**: 28×28 pixels
- **Classes**: 10 digits (0-9)

#### Approach
1. **Data Preprocessing**: Normalization & reshaping for CNN compatibility
2. **Baseline CNN**: Simple convolutional architecture as reference
3. **Enhanced CNN**: Advanced architecture with regularization techniques
4. **Comprehensive Evaluation**: Performance comparison and error analysis

#### Model Architectures
**Baseline CNN**:
- Input (28, 28, 1) → Conv2D(32) → MaxPool → Conv2D(64) → MaxPool → Flatten → Dense(128) → Output(10)

**Improved CNN**:
- Enhanced with Batch Normalization, Dropout layers, and additional convolutional blocks
- Data augmentation: rotation, zoom, shifts, shear transformations
- Early stopping and learning rate scheduling

### 🛠️ Installation & Usage

```bash
# Clone repository
git clone https://github.com/MedAmine-Laouini/Handwriting-Recognition-Task1.git
cd Handwriting-Recognition-Task1

# Install dependencies
pip install -r requirements.txt

# Open and run the notebook in Google Colab
# Upload 'Handwriting_Recognition_Task1.ipynb' to colab.research.google.com
