# rock_vs_mine

This is a simple Machine Learning project that classifies sonar signal data to determine whether the object is a rock or a mine based on the sonar return signal.

📁 Dataset

    Source: UCI Sonar Dataset

    Attributes: 60 numerical features per instance representing energy in various frequency bands.

    Labels:

        R = Rock

        M = Mine

⚙️ Features

    Loads and explores sonar dataset using pandas

    Splits dataset into training and test sets

    Trains a Logistic Regression classifier

    Evaluates accuracy on training and test data

    Predicts for a custom input example

🚀 Getting Started

1. Clone the Repository

git clone https://github.com/asw-beep/rock_vs_mine.git
cd rock_vs_mine

2. Install Dependencies

Make sure you have Python 3 installed. Then install the required libraries:

pip install numpy pandas scikit-learn

3. Add Dataset

Place the Copy of **Copy of sonar data.csv** file in the project directory.
You can download it from the UCI ML Repository.

🧠 How It Works

model = LogisticRegression()
model.fit(X_train, Y_train)

    Preprocessing: Data is split into features (X) and labels (Y).

    Model: Logistic Regression is trained using scikit-learn.

    Prediction: Given a new set of 60 features, the model predicts if it's a rock or a mine.


📊 Results

    Training Accuracy: ~85%

    Test Accuracy: Depends on random state (typical: ~78-90 %)

    ⚠️ Note: The accuracy may vary on different runs.

📦 Input Example

input_data = (0.0762, 0.0666, ..., 0.0094)

    Predicts if the given sonar signal corresponds to a rock or a mine.

    Converts the input into a NumPy array and reshapes it before feeding into the model.

✅ Output Example

['R']
The object is a Rock


<hr>


👨‍💻 Author

Made by Aswin (asw-beep)
