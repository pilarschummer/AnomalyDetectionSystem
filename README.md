# AnomalyDetectionSystem

The network anomaly detection system can be found in the following Github repository [repository-link]. The scripts are organized by system functionalities, including exploratory data analysis, anomaly labeling according to the desired threshold, training and prediction of new data, as well as training of an LSTM for variable prediction.

The execution of the Python scripts is done in a customized way by means of arguments. The user can specify the desired dataset, as well as different parameters such as the classification algorithm to be used (--logistic_regression, --random_forest, --svm), the new data to be introduced to detect whether it is an anomaly or not (--new_data) and the desired metric to be predicted in the prediction script using a LSTM.

The requirements and steps to execute the code are as follows:

1. **Python installation:** The Python programming language must be installed to run the scripts. The latest stable version can be downloaded directly from the website. During installation, the option “Add Python to PATH” should be checked to facilitate command line usage.

2. **Open command terminal:** Once the terminal is open, navigate to the destination directory where the code is to be downloaded:
    ```bash
    cd path/directory/target
    ```

3. **Download the code:** To perform this step you can run the following command which clones the repository:
    ```bash
    git clone https://github.com/user/repository-name.git
    ```

4. **Run the code:** Depending on the desired Python script to be executed, the commands are as follows:
    ```bash
    python labelAnomaly.py dataset.csv # Threshold based anomaly labeling
    python classification.py logistic_regression dataset.csv --new_data 1.0 2.0 3.0 4.0 5.0 6.0 # Detection 
    python predictionLSTM.py dataset.csv throughput # Prediction
    ```

