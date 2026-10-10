# Data
## Data Preparation and Workflow

### 1. Download the Dataset

Download the original **IMS Bearing Dataset** from the official [NASA Open Data Portal](https://data.nasa.gov/dataset/ims-bearings/resource/7adad32f-5984-4a38-b1e3-e0dd2e462dc8). The dataset contains vibration measurements collected from bearings during run-to-failure experiments.

### 2. Raw Data Preprocessing and Feature Extraction

Open and run `Raw data Handling and visualization.ipynb` to process the original raw vibration data. This notebook handles the initial data preparation, signal analysis, and feature extraction required to transform the raw measurements into a structured dataset.

After preprocessing, the notebook generates `ims_features_dataset.csv`, which contains the extracted features used for subsequent machine learning and deep learning experiments.

### 3. Model Development

The processed dataset is used to develop and evaluate different approaches to bearing health monitoring and predictive maintenance, including:

- **Long Short-Term Memory (LSTM):** A recurrent neural network approach for modeling sequential data and predicting bearing degradation.
- **Convolutional Neural Network (CNN):** A deep learning approach for learning patterns from bearing condition data.
- **Random Forest Regression:** An ensemble machine learning method for regression-based prediction.
- **Multivariate Time-Series Forecasting:** A time-series approach for analyzing temporal patterns and forecasting future bearing behavior.

The project explores both machine learning and deep learning techniques to investigate bearing condition monitoring, degradation behavior, and Remaining Useful Life (RUL) prediction.

### 4. Recommended Execution Order

1. Download the original IMS Bearing Dataset from the official source.
2. Place the downloaded data in the appropriate project directory.
3. Run `Raw data Handling and visualization.ipynb` to preprocess the raw data and generate the feature CSV.
4. Use the generated `ims_features_dataset.csv` as the input dataset for the modeling notebooks.
5. Run the relevant notebooks to train and evaluate the different models.

**Note:** The original dataset and generated CSV files are not included in this repository because of their size. You must generate the processed dataset locally before running the modeling notebooks.

