# Driver Drowsiness Detection Using Deep Learning

A real-time driver drowsiness detection system using deep learning and computer vision techniques, developed to enhance road safety by identifying signs of driver fatigue through eye state classification.

---

## Project Overview

This project presents a comparative analysis of multiple deep learning models trained with varying **learning rates** and **optimizers** to improve the accuracy and generalization of driver drowsiness detection systems. The objective is to identify the most effective hyperparameter configuration for reliable, real-time detection of drowsy states in drivers.

---

## Dataset

- **Dataset**: [MRL Eye Dataset](https://mrl.cs.vsb.cz/eyedataset)
- **Subset Used**: 4,000 infrared eye images (open and closed states)
- **Preprocessing**: Images were resized and normalized for input into CNN architectures

---

## Model Training & Experiments

Multiple Jupyter notebooks document training logs and evaluations using different combinations of learning rates and optimizers:

- `DLRTDD_ADAM.ipynb`
- `DL_RTDD_LR0.0001.ipynb`
- `DL_RTDD_LR0.001.ipynb`
- `DL_RTDD_LR0.01.ipynb`
- `DL_RIDD_NADAM.ipynb`
- `DL_RTDD_RMSprop.ipynb`

### Optimizers Evaluated:
- **Adam**
- **RMSProp**
- **Nadam**

### Learning Rates Tested:
- `0.0001`
- `0.001`
- `0.01`

---

## Results Summary

| Optimizer | Learning Rate | Performance | Remarks |
|-----------|----------------|-------------|---------|
| Adam      | 0.001          | Moderate    | Quick convergence but overfitting |
| RMSProp   | 0.001          | High        | Stable and generalizes well |
| Nadam     | 0.001          | Highest     | Smooth convergence and better generalization |

- Lower learning rates resulted in slower training
- Higher learning rates led to faster convergence but risked overfitting
- RMSProp and Nadam provided more stable and reliable training outcomes

### 📈 Comparative Analysis Chart

![Driver Drowsiness Detection Optimizer's Results](https://github.com/boopal2003/Driver-Drowsiness-detection-using-Deep-Learning/blob/main/Screenshot%202025-04-13%20174912.png)
![Driver Drowsiness Detection Learning Rate Results](https://github.com/boopal2003/Driver-Drowsiness-detection-using-Deep-Learning/blob/main/Screenshot%202025-04-13%20180315.png)

![Results](https://github.com/boopal2003/Driver-Drowsiness-detection-using-Deep-Learning/blob/main/Screenshot%202025-04-13%20174842.png)


---

## Tech Stack

- Python
- TensorFlow / Keras
- OpenCV
- Matplotlib
- NumPy
- Jupyter / Google Colab

---

## External Files

Due to GitHub's file size restrictions, the trained `.h5` model files are hosted externally:

📁 [**Access Model Files on Google Drive**](https://drive.google.com/drive/folders/1Umijm-L6V13PSQzLcCS1zyg6rvLyfT3o?usp=sharing) 


---


## Contact

For more information or collaboration opportunities, feel free to get in touch.
