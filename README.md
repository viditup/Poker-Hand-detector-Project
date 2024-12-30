# Poker Hand Detector Project

Welcome to the **Poker Hand Detector Project**! This project is designed to automatically detect poker hands from images of playing cards using machine learning and computer vision techniques. The project employs a deep learning model trained to recognize card suits and values, and then evaluates the poker hand based on those detected values.

---

### **Overview**

The goal of this project is to detect and evaluate poker hands from images of playing cards. This can be particularly useful for automated poker games, card counting, and even for analyzing hands in online poker games.

---

### **Features**
- **Card Detection**: Detects and recognizes playing cards in images using advanced object detection techniques.
- **Poker Hand Evaluation**: Evaluates the poker hand based on the detected cards (e.g., Royal Flush, Straight, Pair).
- **Deep Learning**: Utilizes the YOLO model for object detection and a custom-trained model (`playingcard.pt`) to classify the detected cards.
- **High Accuracy**: Achieves high detection and evaluation accuracy, useful for both real and virtual poker games.

---

### **Tech Stack and Requirements**

This project uses several tools and libraries for optimal performance:

#### **Required Libraries**:
Install the following Python libraries by running:
```bash
pip install -r requirements.txt
```

- **cvzone**: 1.5.6
- **ultralytics**: 8.0.26 (for YOLO models)
- **hydra-core**: >=1.2.0
- **matplotlib**: >=3.2.2
- **numpy**: >=1.18.5
- **opencv-python**: 4.5.4.60
- **Pillow**: >=7.1.2
- **PyYAML**: >=5.3.1
- **requests**: >=2.23.0
- **scipy**: >=1.4.1
- **torch**: >=1.7.0
- **torchvision**: >=0.8.1
- **tqdm**: >=4.64.0
- **filterpy**: 1.4.5
- **scikit-image**: 0.19.3
- **lap**: 0.4.0

#### **System Requirements**:
- **CUDA & GPU Support**: This project uses **CUDA** for GPU acceleration. You will need an NVIDIA GPU with compatible drivers installed.
- **PyTorch with CUDA**: Ensure PyTorch is installed with GPU support:
  ```bash
  pip install torch torchvision torchaudio
  ```

---

### **Project Structure**

```bash
Poker-Hand-Detector/
├── Poker-Hand-Detector.py
├── PokerHandFunction.py
├── playingcard.pt
├── __pycache__/
├── requirements.txt
└── README.md
```

---

### **How to Run the Code**

1. **Install Dependencies**:
   First, install all required libraries by running:
   ```bash
   pip install -r requirements.txt
   ```

2. **Run the Detection Script**:
   - To start poker hand detection, simply run the following command:
   ```bash
   python Poker-Hand-Detector.py
   ```

3. **Input Sources**:
   - For **real-time detection**, you can use a webcam or input image files.
   - For **image-based input**, place the image files in the same directory as the script and update the file path in the code.

4. **Model Weights**:
   - Ensure the correct pre-trained weights (`playingcard.pt`) are available in the same directory as the script.

---

### **Project Demonstrations**

The system detects poker hands by analyzing the suits and ranks of playing cards from input images. The detected poker hand is evaluated and outputted.

#### **Example 1: Poker Hand Detection**

This is an example of how the system detects and evaluates the poker hand from an image of cards.

![Screenshot 2024-12-30 181544](https://github.com/user-attachments/assets/b28c4aa5-7b15-4c78-9680-44017a1bc062)


#### **Example 2: Poker Hand Evaluation**

Another example of a hand being evaluated after detection.

![Screenshot 2024-12-30 181637](https://github.com/user-attachments/assets/d4c6ef7a-9565-493f-bef0-d3124b7ac577)


---

### **Key Files:**
- **`Poker-Hand-Detector.py`**: Main script for detecting playing cards and evaluating poker hands. This script loads the image, processes the card detection, and evaluates the hand.
- **`PokerHandFunction.py`**: A utility script that contains functions for card detection and poker hand evaluation. It uses the YOLO model to detect the cards and then classifies them.
- **`playingcard.pt`**: The pre-trained model used for detecting the playing cards in the image. This model is a YOLO-based object detection model fine-tuned for card recognition.

---

### **Contributing**

We welcome contributions to this project! If you'd like to contribute:

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-name`).
3. Make your changes and test them.
4. Push your changes (`git push origin feature-name`).
5. Open a pull request with a detailed description of your changes.

---

### **License**

This project is licensed under the **MIT License**.

---

### **Acknowledgments**

- **YOLO**: Special thanks to the creators of the YOLO model for their contributions to object detection.
- **OpenCV**: For handling image input and processing.
- **PyTorch**: For deep learning model training and GPU acceleration.

---

### **Contact**

If you have any questions or suggestions, feel free to open an issue in the repository or contact me at viditupadhyay07gmail.com.

