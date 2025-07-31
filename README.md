# Skin Cancer Detection Web App

This project is a Flask-based web application for skin cancer detection using a deep learning model. Users can upload skin lesion images and provide demographic information to receive instant predictions and information about possible skin conditions.

## Features

- Upload skin lesion images for analysis
- Input age, sex, and lesion location
- Get top 3 predicted skin conditions with risk levels, descriptions, and treatment options
- Responsive frontend with instant feedback
- Privacy-focused: no data is stored

## Project Structure

```
app.py
model.h5
requirements.txt
static/
    js/
        prediction.js
        theme.js
    styles/
        main.css
        predict.css
        slider.css
templates/
    index.html
    predict.html
```

## Setup Instructions

1. **Clone the repository**  
   ```
   git clone <your-repo-url>
   cd <project-directory>
   ```

2. **Install dependencies**  
   It is recommended to use a virtual environment.
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. **Add the model**  
   Place your trained Keras model file as `model.h5` in the project root.

4. **Run the app**  
   ```
   python app.py
   ```
   The app will be available at [http://127.0.0.1:5000](http://127.0.0.1:5000).

## Usage

- Go to the home page to learn about skin cancer types.
- Navigate to the prediction page to upload an image and enter your information.
- View the results and recommended next steps.

## Requirements

- Python 3.7+
- See `requirements.txt` for Python package dependencies.

## Notes

- The model expects images resized to 28x28 pixels and user inputs (age, sex, localization) as described in [`app.py`](app.py).
- For best results, use clear, well-lit images of skin lesions.

## License

This project is for educational purposes. Please consult a healthcare professional
