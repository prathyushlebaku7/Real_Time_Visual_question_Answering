# 🌟 Real-Time Visual Question Answering

Welcome to the **Real-Time Visual Question Answering** repository! This project leverages cutting-edge deep learning techniques to answer questions about visual content in real time. By combining object detection and depth estimation, it provides accurate answers to questions based on images.

<img width="922" alt="Screenshot 2025-01-06 at 10 13 42 PM" src="https://github.com/user-attachments/assets/6c01e46c-5d6a-46ec-bd53-26d50ac95906" />

## 📑 Table of Contents
- [✨ Features](#features)
- [📥 Installation](#installation)
- [🚀 Usage](#usage)
- [📂 Project Structure](#project-structure)
- [🔍 Examples](#examples)
- [🤝 Contributing](#contributing)
- [📜 License](#license)

## ✨ Features
- 🕒 **Real-Time VQA**: Answer questions about images instantly.
- 📸 **Object Detection**: Recognizes objects within the image to inform answers.
- 🌄 **Depth Estimation**: Adds depth data to enhance context awareness.
- 🤖 **Model Integration**: Incorporates models like LLava-1.5v-13b for advanced VQA capabilities.

## 📥 Installation

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/prathyushlebaku7/Real_Time_Visual_question_Answering.git
    cd Real_Time_Visual_question_Answering
    ```

2. **Set up the Environment**:
    Ensure you have Python 3.7+ installed. Install dependencies with:
    ```bash
    pip install -r requirements.txt
    ```
    *(Check that a `requirements.txt` file exists; otherwise, manually install dependencies.)*

3. **Download Necessary Models**:
    📦 Download model files for object detection and depth estimation, and place them in the specified directories. Find download links and details [here](#) *(link if available)*.

## 🚀 Usage

1. **Run Object Detection with Depth Estimation**:
    ```bash
    python Object_detection_with_depth/main.py --image <path_to_image>
    ```
    Replace `<path_to_image>` with the path to your image.

2. **Execute Real-Time VQA**:
    ```bash
    python real_time_vqa.py --image <path_to_image> --question "<your_question>"
    ```
    - 🖼️ `--image`: Path to the input image.
    - ❓ `--question`: The question you want to ask about the image.

3. **Using Pre-Trained Models**:
    For LLava-1.5v-13b model predictions, navigate to the `LLava-1.5v-13b_Predictions` folder and follow the specific instructions there.

## 📂 Project Structure

- **Object_detection_with_depth**: Contains scripts for object detection and depth estimation.
- **LLava-1.5v-13b_Predictions**: Tools and files for working with the LLava-1.5v-13b model.
- **README.md**: Documentation for the project.
- **real_time_vqa.py**: Main script for running VQA in real time.

## 🔍 Examples

Here are some usage examples:

```bash
# Example for real-time VQA
python real_time_vqa.py --image examples/sample_image.jpg --question "What is in the image?"

# Expected Output:
# "There is a dog sitting on the grass."
