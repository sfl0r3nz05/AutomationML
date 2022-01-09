# Machine Learning Automation Project

## Working on Jupyter Notebook

### Deploy a Jupyter notebook based on docker

- `docker run -p 8888:8888 jupyter/scipy-notebook:33add21fab64`

- Open a browser with the address that appear once container is deployed:
  - E.g.: `http://127.0.0.1:8888/?token=eec239453d707c8d52fdc180065821c5b21ff26b5b4309f4`.

### Starting with the Data set

- [Download the CSV sample file compressed as a zip file](https://bit.ly/3muqqta).
- Extract the `*.csv` from the zip file.
- Upload the dataset into the Jupyter Notebook.
- The `*.csv` is included in the folder `~/Dataset`

### Create a Model

#### Steps to create a model

- Import the Data
- Clean the Data
- Split the Data into Taining/Test Sets
- Create a Model
- Train the Model
- Make predictions
- Evaluate and improve

- Jupyter Notebook folder contain the `~/Jupyter_Notebook/Create_Model.ipynb` approach.

### Model persistence

#### Export the Model

- Import the library `from joblib import dump`.
- Export the model once it has been trained, e.g.: `dump(model, 'music-recommender.joblib')`.
- Model has been exported into `~/Model`
- Jupyter Notebook folder contain the `~/Jupyter_Notebook/Export_Model.ipynb` approach.

#### Import the Model

- Import the model: `model = load('music-recommender.joblib')`
- Make predictions, e.g.: `predictions = model.predict([[21, 1]])`
- Jupyter Notebook folder contain the `~/Jupyter_Notebook/Import_Model.ipynb` approach.
