# Flask Face Api App

Flask-Face-Api App is a Flask application that utilizes the Face-API.js library which uses TensorFlow.js to detect emotions on faces in real-time using the camera input. This application allows you to perform facial emotion detection locally, reducing compute resource consumption by leveraging the power of TensorFlow.js and integrating it with Flask using websockets. This is an ideal app to be used on devices with very low computational capabilities.

## Table of Contents
- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [How it Works](#how-it-works)
- [Contributing](#contributing)
- [License](#license)

## Introduction
The Face API Python repository is a Flask app that can perform face emotion detection. It utilizes the Face-API.js library, developed by [justadudewhohacks](https://github.com/justadudewhohacks), to perform facial emotion detection. The required models from Face-API.js are downloaded and used locally in this repository.

## Prerequisites
Before you can use Face API Python, please ensure that the following prerequisites are met:
- Python 3.6 or later is installed on your machine.
- A webcam or camera connected to your computer.

## Installation
To install and set up the Face API Python application, follow these steps:

1. Clone the repository using the following command:
    ```bash
    git clone https://github.com/manish-9245/flask-face-api.git
    ```

2. Change to the cloned directory:
    ```bash
    cd flask-face-api
    ```

3. Install the required Python packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
To use the Flask Face Api application, follow these steps:

1. Start the Flask server by running the following command:
    ```bash
    python application.py
    ```

2. Once the server is running, open your web browser and navigate to `http://localhost:5000`.

3. Grant permission to access your camera when prompted by the browser.

4. The application will automatically detect faces in the camera input and display the corresponding emotions in real-time.

## How it Works
The Face API Python application utilizes Flask, a web framework for Python, to host a web server. It also utilizes the MediaDevices API and Canvas API provided by modern web browsers to capture the camera input and display the results in real-time.

When the web page is loaded, it establishes a websocket connection with the Flask server. The server continuously captures frames from the camera input and performs facial emotion detection using the Face-API.js library and TensorFlow.js. The results are then sent back to the client through the websocket connection and displayed on the web page.

The Face-API.js library provides pre-trained models for facial detection and emotion classification, which are downloaded and used locally in this repository.

## Contributing
Contributions to the Face API Python repository are welcome. If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## License
This repository is licensed under the MIT License. Please see the [LICENSE](LICENSE) file for more information.