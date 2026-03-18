<img width="1897" height="970" alt="image" src="https://github.com/user-attachments/assets/ad7af0d9-180d-423a-bcaf-055fcb11329a" />
This the plateform view 

# Car Insurance Claim Prediction - Flask App

## Project structure
- `app.py` : Flask backend
- `train_and_export_model.py` : trains and exports the model bundle
- `templates/index.html` : frontend page
- `static/style.css` : styling
- `static/script.js` : frontend logic
- `requirements.txt` : dependencies
- `car_insurance.csv` : dataset
- `model_bundle.joblib` : exported model, scaler, and feature names

## How to run in Visual Studio Code
1. Open the folder in VS Code.
2. Create a virtual environment:
   - `python -m venv venv`
3. Activate it:
   - Windows: `venv\\Scripts\\activate`
4. Install dependencies:
   - `pip install -r requirements.txt`
5. Put `car_insurance.csv` inside the project folder.
6. Train and export the model:
   - `python train_and_export_model.py`
7. Start the Flask app:
   - `python app.py`
8. Open your browser at:
   - `http://127.0.0.1:5000`

## Notes
- The app uses Logistic Regression.
- Categorical values are encoded with `pd.get_dummies()`.
- Input columns are aligned with training columns using `reindex()`.
