# Video-Games-Recommender-Using-NMF-Collaborative-Filtering

This *Collaborative Filtering-based Video Games Recommender System* focuses on *Non-Negative Matrix Factorization (NMF)*. This project used a dataset from **Kaggle** [Steam Video Games](https://www.kaggle.com/datasets/tamber/steam-video-games "Get Dataset Here") for training and another dataset that is also from Kaggle [Steam Store Games (Clean dataset)](https://www.kaggle.com/datasets/tamber/steam-video-games "Get Dataset Here") for the metadata of the games. 

## Installation  

### Installation Steps  

1. **Clone this repository**  
   ```
   git clone https://github.com/Tuanwaf/Video-Games-Recommender-using-NMF-Collaborative-Filtering.git
   ```
   
2. **Enter the project directory**
   ```
   cd Video-Games-Recommender-Using-NMF-Collaborative-Filtering
   ```
   
3. **Install dependencies**
   ```
   pip install -r requirements.txt
   ```

   Or you can also directly install the requirement in **Jupyter Notebook** cell:
   
   ```
   !pip install -r requirements.txt
   ```

## Important

This project was run in **Jupyter Notebook**. If you want the same experience, consider using this environment too.

## Run the project

1. Open your **Jupyter Notebook**, make sure you have install the ```requirements.txt```
2. You can see some of the datasets used inside the ```/data``` folder. This is because some data are too big to be put here. You need to download the dataset for metadata by yourself from the link above and put it into the ```/data``` folder.
3. Run all these files in sequence:
   - ```Dataset_Cleaning.ipynb``` This is where you will clean the dataset to be used during the training.
   - ```Dataset_Combined.ipynb``` This merges the cleaned dataset with the games' metadata, such as genre, description, and so on.
   - ```NMF_Model.ipynb``` This is the actual *Collaborative Filtering* model used for the training.
   - ```Evaluation.ipynb``` This is the evaluation process for the CF model; it uses RMSE, MAE, and Recall@K.
   - ```Streamlit_main.ipynb``` This is to run the streamlit interface, but before running this, make sure to check the interface code at ```interface.py```; you can edit the interface code here.
