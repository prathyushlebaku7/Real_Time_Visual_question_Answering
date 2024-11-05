# Real-Time Visual Question Answering

This repository provides an implementation of real-time visual question answering (VQA) using deep learning techniques. The project leverages object detection and depth estimation models to process images, enabling real-time responses to questions based on visual input.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)

## Features
- **Real-Time VQA**: Answer questions about images in real-time.
- **Object Detection**: Identifies objects in images to provide context-aware answers.
- **Depth Estimation**: Uses depth information to improve accuracy and context in answers.
- **Model Integration**: Integrates with LLava-1.5v-13b and other models for advanced VQA capabilities.

## Installation

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/prathyushlebaku7/Real_Time_Visual_question_Answering.git
    cd Real_Time_Visual_question_Answering
    ```

2. **Set up the Environment**:
    Ensure you have Python 3.7+ installed. Install required packages with:
    ```bash
    pip install -r requirements.txt
    ```
    *(Ensure that a `requirements.txt` file is in the repository; if not, list dependencies manually.)*

3. **Download Necessary Models**:
    Download and place model files for object detection and depth estimation in the appropriate directories. Model download links and instructions can be found [here](#) *(add link if available)*.

## Usage

1. **Run Object Detection with Depth Estimation**:
    ```bash
    python Object_detection_with_depth/main.py --image <path_to_image>
    ```
    Replace `<path_to_image>` with the path to your image file.

2. **Execute Real-Time VQA**:
    ```bash
    python real_time_vqa.py --image <path_to_image> --question "<your_question>"
    ```
    - `--image`: Path to the input image.
    - `--question`: The question you want to ask about the image.

3. **Using Pre-Trained Models**:
    To use the LLava-1.5v-13b model predictions, navigate to the `LLava-1.5v-13b_Predictions` folder and follow the instructions provided.

## Project Structure

- **Object_detection_with_depth**: Contains scripts for object detection and depth estimation.
- **LLava-1.5v-13b_Predictions**: Includes files and tools related to the LLava-1.5v-13b model.
- **README.md**: Documentation for the project.
- **real_time_vqa.py**: Main script for running visual question answering in real-time.

## Examples

Below are some example commands and expected outputs.

```bash
# Example command for real-time VQA
python real_time_vqa.py --image examples/sample_image.jpg --question "What is in the image?"

# Expected Output:
# "There is a dog sitting on the grass."

![image](https://github.com/user-attachments/assets/1b5624c6-fdad-47eb-825b-29b27ce8fb3b)
