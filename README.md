**Fire** **Weather** **Index** **(FWI)** **Prediction** **System**

A Flask-based web application that predicts Fire Weather Index (FWI)
using machine learning. The system uses a Ridge Regression model to
predict fire weather conditions based on various meteorological and
environmental parameters.

🔥 **Features**

> **Web-based** **Interface**: User-friendly form for inputting weather
> parameters
>
> **Machine** **Learning** **Prediction**: Uses trained Ridge Regression
> model for accurate FWI predictions
>
> **Real-time** **Results**: Instant prediction results displayed on the
> web interface
>
> **Robust** **Error** **Handling**: Comprehensive error handling for
> reliable operation
>
> **Responsive** **Design**: Clean and modern web interface

📋 **Requirements**

> Python 3.7+
>
> Flask
>
> scikit-learn
>
> pandas
>
> numpy
>
> pickle

🚀 **Installation**

> 1\. **Clone** **the** **repository:**
>
> bash
>
> git clone https://github.com/Shreyann05/ML-Project.git cd
> fwi-prediction-app
>
> 2\. **Create** **a** **virtual** **environment** **(recommended):**
>
> bash
>
> python -m venv venv
>
> source venv/bin/activate *\#* *On* *Windows:* *venv\Scripts\activate*
>
> 3\. **Install** **required** **packages:**
>
> bash
>
> pip install -r requirements.txt
>
> 4\. **Ensure** **the** **following** **directory** **structure:**
>
> fwi-prediction-app/ ├── app.py
>
> ├── models/
>
> │ ├── ridge.pkl │ └── scaler.pkl ├── templates/
>
> │ ├── index.html │ └── home.html ├── requirements.txt └── README.md

🎯 **Usage**

> 1\. **Start** **the** **Flask** **application:**
>
> bash
>
> python app.py
>
> 2\. **Open** **your** **web** **browser** **and** **navigate** **to:**
>
> http://localhost:5000
>
> 3\. **Enter** **the** **required** **parameters:** **Temperature**:
> Temperature in Celsius
>
> **RH**: Relative Humidity (%)
>
> **Ws**: Wind Speed (km/h)
>
> **Rain**: Rainfall (mm)
>
> **FFMC**: Fine Fuel Moisture Code
>
> **DMC**: Duff Moisture Code
>
> **ISI**: Initial Spread Index
>
> **Classes**: Fire Weather Class
>
> **Region**: Region Code
>
> 4\. **Click** **"Predict** **FWI"** to get the Fire Weather Index
> prediction

🧠 **Model** **Information**

> **Algorithm**: Ridge Regression
>
> **Preprocessing**: StandardScaler for feature normalization
>
> **Input** **Features**: 9 meteorological and environmental parameters
>
> **Output**: Fire Weather Index (FWI) prediction

📁 **File** **Structure**

> ├── app.py \# Main Flask application ├── models/
>
> │ ├── ridge.pkl
>
> │ └── scaler.pkl

\# Trained Ridge Regression model

\# StandardScaler for data preprocessing

> ├── templates/
>
> │ ├── index.html
>
> │ └── home.html

\# Landing page template

\# Main prediction form and results page

> ├── requirements.txt
>
> └── README.md
>
> \# Python dependencies

\# Project documentation

🔧 **API** **Endpoints**

> **GET** **/**: Home page
>
> **GET** **/predictdata**: Prediction form page
>
> **POST** **/predictdata**: Submit prediction request and get results

🛠 **Development**

**Running** **in** **Debug** **Mode**

> bash
>
> python app.py

The application runs with debug mode enabled for development.

**Model** **Training**

The pre-trained models ( ridge.pkl and scaler.pkl) are included in the
models/ directory. If you need to retrain the models:

> 1\. Prepare your training data with the same 9 features
>
> 2\. Train a Ridge Regression model
>
> 3\. Fit a StandardScaler on the training data
>
> 4\. Save both models using pickle in the models/ directory

🚨 **Error** **Handling**

The application includes comprehensive error handling for:

> Missing model files
>
> Invalid input data
>
> Form submission errors
>
> Template rendering issues

🌐 **Deployment**

**Local** **Deployment**

The app is configured to run on 0.0.0.0 making it accessible on your
local network.

**Production** **Deployment**

For production deployment, consider:

> Using a production WSGI server (e.g., Gunicorn)
>
> Setting up proper environment variables
>
> Implementing additional security measures
>
> Setting up logging

📊 **Input** **Parameters** **Explanation**

> **Temperature**: Ambient temperature (°C)
>
> **RH**: Relative humidity percentage
>
> **Ws**: Wind speed (km/h)
>
> **Rain**: Precipitation amount (mm)
>
> **FFMC**: Fine Fuel Moisture Code - represents moisture content of
> fine fuels
>
> **DMC**: Duff Moisture Code - represents moisture content of
> decomposed organic matter
>
> **ISI**: Initial Spread Index - indicates the expected rate of fire
> spread
>
> **Classes**: Fire weather classification
>
> **Region**: Geographical region identifier

🤝 **Contributing**

> 1\. Fork the repository
>
> 2\. Create a feature branch ( git checkout -b feature/new-feature)
>
> 3\. Commit your changes ( git commit -m 'Add new feature')
>
> 4\. Push to the branch ( git push origin feature/new-feature)
>
> 5\. Open a Pull Request

📝 **License**

This project is open source and available under the [<u>MIT
License</u>](https://claude.ai/chat/LICENSE).


