---

# **Skin Disease Diagnosis System**

This project is a web-based application that enables users to upload images for detecting and diagnosing common skin diseases using machine learning and image processing techniques. It also includes user authentication, registration, and personalized profiles.

---

## **Features**

- **User Authentication**: Secure login and registration system with validation.
- **Image Upload**: Upload skin images for disease detection.
- **Skin Disease Detection**: Uses a trained machine learning model for diagnosing skin conditions.
- **Diagnosis Details**: Provides treatment suggestions and educational information for detected diseases.
- **User Dashboard**: Personalized profile with uploaded images and diagnosis history.
- **Frontend and Backend Integration**: Built with Django, OpenCV, and Scikit-learn.

---

## **Technologies Used**

### **Frontend**:
- HTML5, CSS3
- Bootstrap for responsive design

### **Backend**:
- Python (Django Framework)
- Django Forms for validation and user authentication
- File Storage for image uploads

### **Machine Learning**:
- Scikit-learn for model training and prediction
- Pre-trained Voting Ensemble model (`voting_ensemble_skin_disease_model.joblib`)

### **Image Processing**:
- OpenCV for feature extraction
- Histogram Equalization, Color Histograms, and HOG Features

---

## **Project Setup**

### **Prerequisites**:
- Python 3.9 or higher
- Virtual Environment (recommended)

### **Installation**:
1. Clone the repository:
   ```bash
   git clone https://github.com/<username>/skin-disease-diagnosis.git
   cd skin-disease-diagnosis
   ```
2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### **Run the Application**:
1. Apply database migrations:
   ```bash
   python manage.py migrate
   ```
2. Start the development server:
   ```bash
   python manage.py runserver
   ```
3. Open your browser and go to `http://127.0.0.1:8000/`.

---

## **Usage**

1. **Registration**: Create an account with a valid username and password.
2. **Login**: Access the system using your credentials.
3. **Upload Image**: Navigate to the profile page and upload an image of the skin condition.
4. **Diagnosis**: View the detected disease and its corresponding diagnosis and treatment information.

---

## **Machine Learning Model**

- **Model Used**: Voting Ensemble Classifier
- **Feature Extraction**:
  - Histogram of Oriented Gradients (HOG)
  - Color Histograms (RGB and HSV)
- **Scalers**: RobustScaler for feature normalization
- **Accuracy**: Achieved **0.80% accuracy** during testing.

---

## **Project Structure**

```plaintext
skin-disease-diagnosis/
├── demopage/                # Main application folder
│   ├── views.py             # Contains view logic
│   ├── models.py            # Database models (if used)
│   ├── forms.py             # Django forms for validation
│   ├── templates/           # HTML templates
├── static/                  # Static assets (CSS, JS, images)
├── media/                   # Uploaded images
├── sample/                  # Project configuration
│   ├── settings.py          # Django settings
│   ├── urls.py              # Project-level URLs
├── manage.py                # Django management script
└── requirements.txt         # Python dependencies
```

---

## **Contributing**

Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add a feature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-name
   ```
5. Open a pull request.

---

## **License**

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## **Acknowledgments**

- Special thanks to the open-source community for tools and libraries like Django, OpenCV, and Scikit-learn.
- Inspiration for skin disease detection sourced from medical image analysis research.

---
