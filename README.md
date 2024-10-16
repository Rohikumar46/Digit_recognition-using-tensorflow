# Handwritten Digit Recognition WebApp

This repository contains a web application that uses a convolutional neural network (CNN) model trained on the MNIST dataset to recognize handwritten digits. The model is run in the browser using TensorFlow.js.

## Table of Contents
- [Project Structure](#project-structure)
- [Running the WebApp Locally](#running-the-webapp-locally)
- [How It Works](#how-it-works)
- [Requirements](#requirements)

## Project Structure

```plaintext
.
├── index.html              # Main HTML file for the web app
├── css/
│   └── styles.css          # CSS file for styling the web app
├── js/
│   └── main.js             # JavaScript for handling user interactions and model predictions
├── model.ipynb             # Jupyter Notebook for training the CNN model on MNIST dataset
└── README.md               # Documentation for the project

```
## File Descriptions:
- **index.html**: The main web page that includes the layout, buttons, canvas for digit drawing, and areas to show predictions.
- **css/styles.css**: Styles for the web page including fonts, layout, and canvas appearance.
- **js/main.js**: The core JavaScript file that handles drawing on the canvas, passing the image to the model, and displaying the prediction results.
- **model.ipynb**: A Jupyter Notebook that trains the CNN on the MNIST dataset, which can later be converted into a TensorFlow.js model for the web.
- **README.md**: The documentation you are reading now.

## How It Works
1. The **canvas** allows users to draw a digit using their mouse.
2. When the **Predict** button is clicked, the drawn image is passed through a pre-trained CNN model, loaded via TensorFlow.js.
3. The app then displays the predicted digit and the model's confidence level.

## Requirements
- **TensorFlow.js** is used for running the model in the browser.
- **Bootstrap 4** and custom **CSS** for the user interface.
- **JavaScript (main.js)** for handling the model and user inputs.

You can install the necessary libraries if you're running this locally:

```bash
npm install @tensorflow/tfjs
```
## Running the WebApp Locally

To run the web app on your local machine, follow these steps:

### 1. Clone the Repository
First, clone the repository to your local machine:

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```






## 2. Run a Local Server
To view the web app, you'll need to serve the files locally. You can do this using Python's built-in HTTP server or a VSCode Live Server.

### Option A: Using Python's SimpleHTTPServer
If you have Python installed, open a terminal in the project directory and run:

```bash
# For Python 3
python -m http.server
```
