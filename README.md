# Water-Potability-Analysis
This project utilizes data visualization and machine learning tools to gain insight into water potability data. The goal is to analyze the physical and chemical properties of water samples to determine whether or not they are safe to drink.

The [potability data][dataset] was downloaded from Kaggle in csv format. It contained 9 continuous feature variables (water properties) and 1 binary target variable (potability). This dataset was split into training (80%) and test (20%) sets.

Five types of binary classifier models were fitted to the training data:
- Logistic Regression
- SVM
- Small Random Forest (10 estimators)
- Large Random Forest (100 estimators)
- XGBoost

The SVM model had the best test accuracy (~70%).

## How to use
1. Clone the repository by running the command `git clone https://github.com/Nielam-Dass/Water-Potability-Analysis.git`.
2. While in the project folder, create a virtual environment of your choice. This process may vary depending on your operating system. On Windows, run `python -m venv venv`, to create an environment folder named `venv`.
3. Activate the environment with `venv\Scripts\activate.bat`.
4. Once the environment is active, install the necessary packages with `pip install -r requirements.txt`.
5. Go to the [Kaggle][kaggle] website and generate an API token, which will be downloaded in JSON format. The file will contain values for the `username` and `key` fields.
6. Create a `.env` file in the project folder, which will define the environment variables `KAGGLE_USERNAME="your_username"` and `KAGGLE_KEY="your_key"` according to the downloaded JSON data.
7. At this point, you can run the Jupyter notebook and make changes to create new models.

[dataset]: https://www.kaggle.com/datasets/nayanack/water-probability
[kaggle]: https://www.kaggle.com/
