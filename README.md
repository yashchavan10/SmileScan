# SmileScan: Predictive Dental Detection

## Overview

SmileScan is a comprehensive system designed to address dental issues in underserved rural areas. By combining advanced machine learning models with an intuitive web interface, SmileScan facilitates early detection and diagnosis of common dental problems. This system aims to improve oral health outcomes by providing timely and accurate assessments, thus overcoming barriers like financial constraints and geographical isolation that often hinder access to dental care.

## Introduction

In rural areas, common dental anxieties and limited transportation options deter people from seeking timely care, leading to neglected early signs of dental issues. SmileScan aims to address this problem by providing an accessible, user-friendly system for early dental issue detection.

## Features

- **Image Capture**: A physical camera device captures oral images and stores them in a database.
- **Web Application**: Integrated with a classifier to diagnose dental issues and provide a questionnaire for additional information.
- **Preliminary Medical Report**: Combines image analysis and questionnaire responses to generate a report with diagnosis and temporary relief recommendations.
- **Medication Dispensing**: Administered by pharmacists based on the generated report.

## System Architecture

1. **Image Capture**: A high-resolution camera device captures images of the patient's oral cavity, along with a desktop application which is used to capture the image
2. **Data Storage**: Images are stored securely in a database.
3. **Web Application**: Interfaces with the classifier and questionnaire module.
4. **Diagnosis**: Utilizes machine learning models to classify dental conditions into six types.

## Technology Stack

- **Front-End**: HTML, CSS, JavaScript
- **Back-End**: Django
- **Database**: MongoDB/SQL
- **Machine Learning Models**: YOLOv8
- **Image Capture GUI**: Tkinter

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-repo/SmileScan.git
    cd Smilescan-Dental-Prediction
    ```

2. **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Set up the database**:
    - Configure your database settings in `settings.py`.
    - Run migrations:
    ```bash
    python manage.py migrate
    ```

4. **Start the server**:
    ```bash
    python manage.py runserver
    ```

## Usage

1. **Image Capture**: Use the designated camera device to capture oral images. Open UploadPhoto.exe to capture images from the camera device.
2. **Upload Image**: Upload the captured images to the web application.
3. **Complete Questionnaire**: Fill out the questionnaire on the web application.
4. **Receive Report**: View the preliminary medical report generated by the system.
5. **Medication Dispensing**: Obtain recommended medications from the pharmacist.

