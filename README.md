🧠 Background Removal using U-Net & ONNX Runtime

This project demonstrates how to remove and replace image backgrounds using deep learning–based segmentation (U-Net architecture) optimized with ONNX Runtime for efficient inference.
It primarily uses the rembg
 library, which leverages a U-Net model exported to ONNX format for real-time background removal.

🚀 Features

U-Net segmentation for accurate background detection

ONNX Runtime for fast and portable inference

Automatic background removal via the rembg library

Custom background replacement (example: green screen)

Simple and lightweight — only a few lines of code

| Component        | Purpose                                                           |
| ---------------- | ----------------------------------------------------------------- |
| **Python 3.x**   | Core programming language                                         |
| **rembg**        | Handles background removal using a pretrained U-Net model         |
| **onnxruntime**  | Runs the deep learning model efficiently without heavy frameworks |
| **Pillow (PIL)** | Image manipulation and saving                                     |
| **NumPy**        | Pixel-level operations for custom background replacement          |


🧬 How It Works

U-Net Architecture
The rembg library uses a U-Net deep learning model — a convolutional network designed for image segmentation.
It identifies the foreground (subject) and background (non-subject) regions pixel by pixel.

ONNX Runtime
The model is exported to ONNX (Open Neural Network Exchange) format, which allows fast, cross-platform inference without needing full frameworks like TensorFlow or PyTorch.

Post-processing
Once the subject is isolated, you can:

Keep a transparent background, or

Replace it with a custom color, pattern, or new image.

| Feature   | Benefit                                                         |
| --------- | --------------------------------------------------------------- |
| **U-Net** | High-accuracy segmentation for background/foreground separation |
| **ONNX**  | Framework-independent, faster inference                         |
| **rembg** | Pre-trained model ready to use, no training required            |

📜 License

This project is open-source under the MIT License.
Based on rembg
