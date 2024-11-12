# VibeSync - Facial Emotion-Based Music Recommendation System

VibeSync is an interactive application that analyzes a user's facial expression to recognize their emotion and recommends mood-specific music. It utilizes a Convolutional Neural Network (ResNet50) for emotion recognition and uses a curated music dataset to suggest suitable songs based on the detected mood. The application is built using Gradio for the user interface and TensorFlow and Keras for machine learning.
VibeSync is an interactive application that analyzes a user's facial expression to recognize their emotion and recommends mood-specific music. It leverages a Convolutional Neural Network (ResNet50) for emotion recognition and uses a curated music dataset to suggest suitable songs based on the detected mood. The application is built using Gradio for the user interface and TensorFlow and Keras for machine learning.

---

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Overview](#overview)
- [Key Features](#key-features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [File Structure](#file-structure)
- [Model](#model)
- [Data](#data)
- [Technologies Used](#technologies-used)
---

## Project Overview
## Overview

VibeSync allows users to upload an image of themselves to detect their mood and get music recommendations that match their emotional state. By leveraging computer vision and a deep learning model, the app provides a seamless and personalized music experience.
VibeSync allows users to upload an image of themselves to detect their mood and receive music recommendations that match their emotional state. By leveraging computer vision and a deep learning model, the app provides a seamless and personalized music experience.

## Features
- **Emotion Detection**: Recognizes emotions such as 'happy,' 'sad,' 'neutral,' 'angry,' and 'fear.'
- **Music Recommendation**: Recommends mood-specific songs based on the detected emotion.
## Key Features
- **Emotion Detection**: Identifies emotions such as 'happy,' 'sad,' 'neutral,' 'angry,' and 'fear.'
- **Music Recommendation**: Suggests mood-specific songs based on the detected emotion.
- **User-Friendly Interface**: Built with Gradio for a smooth user experience.

## Installation

## Getting Started
### Prerequisites
- Python 3.8+
- TensorFlow
- Gradio
- Keras
- OpenCV
- Pandas

### Setup
### Installation
1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/vibesync.git
   cd vibesync

2. **Install the required dependencies**: 
   ```bash
   pip install -r requirements.txt

3. **Download the pre-trained model**: Ensure the `Final_ResNet50_Model.keras` file is located in the root directory.

4. **Prepare the Dataset**: Place `songs_mood.csv` in the root directory. This file should contain columns for song names, artist names, Spotify track IDs, and mood labels.


### Usage
1. **Launch the Application**:
   ```bash
   python app.py

2. **Upload an Image**: Use the Gradio interface to upload your image.

3. **Get Emotion and Recommendations**: The app will display the detected emotion and provide a list of mood-specific song recommendations.

## File Structure
```bash
vibesync/
├── app.py                     # Main application file
├── Final_ResNet50_Model.keras # Pre-trained emotion detection model
├── songs_mood.csv             # Music dataset with mood labels
├── README.md                  # Project documentation
└── requirements.txt           # Required libraries
```

## Model
The emotion detection model used in VibeSync is a Convolutional Neural Network (CNN) based on the ResNet50 architecture. The model has been trained on a dataset of facial expressions to recognize emotions such as 'happy,' 'sad,' 'neutral,' 'angry,' and 'fear.'

## Data
The music dataset used for song recommendations is a curated collection of songs with mood labels. The dataset includes columns for song names, artist names, Spotify track IDs, and mood labels.

## Technologies Used
- Python: Core language for development
- TensorFlow & Keras: Model training and loading
- Gradio: Web-based UI for interactive user experience
- Pandas: Data handling for song recommendations
- OpenCV & PIL: Image processing

