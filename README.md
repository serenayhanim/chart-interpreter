# chart-interpreter

## Overview

**Chart Interpreter** is a Streamlit-based web application designed to help users interpret charts or graphs. By leveraging OpenAI's API, this tool allows users to upload an image of a chart and receive a detailed interpretation as if from an experienced health data analyst. This is particularly useful for stakeholders who need to understand complex visual data.

## Features

- **Image Upload**: Users can upload a chart image in PNG, JPG, or JPEG format.
- **Chart Interpretation**: The app sends the uploaded image to OpenAI's API, which returns an interpretation of the chart, providing insights and explanations.
- **User-Friendly Interface**: The app provides a simple and intuitive interface for easy interaction.

## Running Locally

If you want to run the **Chart Interpreter** app locally, follow these steps:

### Prerequisites

Ensure that you have the following installed on your machine:

- Python 3.7+
- pip (Python package installer)

### Clone the Repository

First, clone the repository to your local machine:

```bash
git clone https://github.com/yourusername/chart-interpreter.git
cd chart-interpreter
```

### Create a Virtual Environment
It's recommended to create a virtual environment to manage the dependencies for this project. You can create and activate a virtual environment using the following commands:

```bash
python -m venv venv
venv\Scripts\activate
```

### Install Dependencies
Once the virtual environment is activated, install the necessary dependencies:

```bash
pip install -r requirements.txt
```
### Set Up OpenAI API Key

To use the OpenAI API, you need to set up your API key. You can do this by:

Creating a .env file in the root directory of your project.

Adding your API key to the .env file:

```bash
OPENAI_API_KEY=your_openai_api_key_here
```
Alternatively, you can use Streamlit's secrets management by creating a secrets.toml file in the .streamlit/ directory and adding your API key:

```bash
[openai]
api_key = "your_openai_api_key_here"
```

### Run the Application
With everything set up, you can now run the Streamlit application:

```bash
streamlit run app.py
```

This command will start a local web server, and the app will open in your default web browser at http://localhost:8501.

### Deployment on Streamlit Cloud
I have also deployed this app on Streamlit Cloud, making it easy to access without running it locally. You can visit the deployed app using the following link:

[chart-interpreter](https://b2fpnouqndyr3jwpzzwvig.streamlit.app/)

