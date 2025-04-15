# 🌿 Plant Disease Detection System for Sustainable Agriculture

A Deep Learning-powered web application that enables early and accurate plant disease diagnosis from leaf images, supporting farmers in adopting sustainable agricultural practices.

## Project Overview

This project uses a **Convolutional Neural Network (CNN)** trained on a dataset of healthy and diseased plant leaf images. The model is deployed via a **Streamlit web application**, allowing users to upload plant leaf images and receive instant predictions about potential diseases.

---

## Features

- Upload a plant leaf image
- Predicts from 35+ disease classes
- Built using TensorFlow and Streamlit
- Offline model inference – no internet needed for predictions
- Easy-to-use interface tailored for non-technical users

---

## Tech Stack

- **Frontend**: Streamlit
- **Backend**: Python, TensorFlow, Keras
- **Model**: CNN trained on the [PlantVillage dataset](https://www.tensorflow.org/datasets/catalog/plant_village)
- **Libraries**: NumPy, PIL, TensorFlow

---

## Sample Output

| Input Leaf Image | Prediction |
|------------------|------------|
| Corn leaf with rust | `Corn_(maize)___Common_rust_` |
| Tomato leaf with curl | `Tomato___Tomato_Yellow_Leaf_Curl_Virus` |

---

## How to Run the Project Locally

1. **Clone the repository**
   ```bash
   git clone https://github.com/Ashwitha-Rudrawalambi/Plant-Disease-Detection-System-for-Sustainable-Agriculture
   cd Plant-Disease-Detection-System-for-Sustainable-Agriculture
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the application**
   ```bash
   streamlit run app.py
   ```

---

## Directory Structure

```
plant-disease-detection/
│
├── trained_plant_disease_model.keras   # Pre-trained model
├── app.py                              # Streamlit application code
├── Diseases.png                        # Banner image
├── requirements.txt                    # Python dependencies
└── README.md                           # Project overview
```

---

## Model Classes

Includes diseases such as:
- Apple Scab
- Tomato Mosaic Virus
- Corn Rust
- Potato Blight
- ...and many more (35+ total)

---

## Limitations

- Sensitive to image quality (blurred or low-light images may reduce accuracy)
- Predictions are limited to known classes in the dataset
- Does not currently suggest treatments

---

## Future Enhancements

- Integration with IoT devices and drones for field deployment
- Mobile app development for better accessibility
- Support for region-specific crops
- Use of advanced architectures like EfficientNet or Vision Transformers
- Explainability tools (e.g., Grad-CAM for visual insights)
