# Real-Time Face Mask Detection System
This project is a real-time face mask recognition system that detects whether individuals in live video streams are wearing masks or not. It leverages transfer learning with a pre-trained MobileNetV2 model and OpenCV for video capture and processing.

## Project Demo 
https://github.com/Ishita2407/Face-mask-Detector-/assets/91796142/fde59d8b-13e2-4063-8fc0-f632684d2546

## Features
- **Real-time detection** of face masks in live video streams.
- Built using **MobileNetV2** with transfer learning for efficient performance.
 ![image](https://github.com/user-attachments/assets/e84f9cc2-74b2-49d5-8aad-734c98e5e8e0)

- Custom fully connected layers for **binary classification**: 'with mask' and 'without mask'.
  ![image](https://github.com/user-attachments/assets/fe257c6b-4a4d-4b22-bcba-e0ebc47ec6b0)

- Achieved **90% precision** and an **F1 score of 92%**.
- Applied **data augmentation** for robust model training.

## How It Works
1. **Model**: Transfer learning is used with **MobileNetV2**, a lightweight CNN model pre-trained on ImageNet.
   Image net Architecture:
   ![image](https://github.com/user-attachments/assets/416938ee-8019-4a84-8537-bc2c119eaf0e)

3. **Fine-tuning**: Custom fully connected layers are added for the specific task of mask detection.
4. **Preprocessing & Augmentation**: Input images are preprocessed and augmented (rotation, flipping, etc.) to improve model robustness.
  ![image](https://github.com/user-attachments/assets/bca62d16-ce7e-4e62-b040-e1385130ad2d)

6. **Real-time Video Processing**: OpenCV captures video and detects faces, passing them through the trained model for classification.

## Technologies Used
- **Python**: Core programming language.
- **TensorFlow / Keras**: For model training and transfer learning.
- **OpenCV**: For real-time video processing and face detection.
- **MobileNetV2**: Pre-trained model for transfer learning.

## Results
- **Precision**: 90%
- **F1 Score**: 92%
- **Real-time performance**: Detects mask status in live video streams.

## Dataset
The model was trained using a custom dataset containing images of people with and without masks, and was augmented for better performance in varied conditions.

## Future Enhancements
- Expand to multi-class classification to detect incorrectly worn masks.
- Improve performance on edge devices by further optimizing the model.
- Integrate with IoT devices for real-world deployment (e.g., in offices, public spaces).

## Contributing
Feel free to fork this project, submit issues, and make pull requests!
