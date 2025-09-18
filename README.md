# Shape Classifier

A lightweight CNN model for classifying geometric shapes using TensorFlow Lite.

## Features
- Classifies 4 shapes: circle, rectangle, square, triangle
- 64x64 pixel input images
- Optimized TensorFlow Lite model for mobile/embedded deployment
- Simple training pipeline

## Setup

### Install Dependencies
```bash
pip install tensorflow pillow numpy matplotlib
```

### Dataset Structure
Organize your images in the following structure:
```
dataset/
└── train/
    ├── circle/
    │   ├── image1.jpg
    │   └── image2.jpg
    ├── rectangle/
    │   ├── image3.jpg
    │   └── image4.jpg
    ├── square/
    │   ├── image5.jpg
    │   └── image6.jpg
    └── triangle/
        ├── image7.jpg
        └── image8.jpg
```

## Usage

1. **Prepare your dataset** with at least 20-50 images per shape category
2. **Run the Jupyter notebook** to train the model
3. **Get your optimized model** - `model.tflite` file ready for deployment

## Model Details
- **Input:** 64x64 RGB images
- **Output:** 4 classes (circle, rectangle, square, triangle)
- **Architecture:** Simple CNN with 3 convolutional layers
- **Training:** 50 epochs, batch size 64

## Files Generated
- `model.tflite` - Optimized TensorFlow Lite model
- Training logs and accuracy metrics

## Testing
The notebook includes code to test your model with new images and shows prediction confidence percentage.

---
*Built with TensorFlow Lite for efficient shape recognition*