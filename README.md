# Multi-label Movie Genres Classification

## Project Description
### Dataset
The dataset for this project is compressed in "dataset.zip" which has:
1. ml1m-images folder which contains the movie cover images/posters, the name of the image is the id of the movies it associates
2. genres.txt file contains every possible genres in training and test data
3. movies_{train|test}.dat: training and testing files, containing the information of the movies, for example the id, name, and its genres
4. ratings.dat: data file containing the ratings of user-movie pairs.
5. users.dat: data file containing the information of the users.

**Note:** For more detail about each field in the data files, please read the "data_description.txt"

### Models
The 2 models used in this project:
1. The pre-trained BERT model is used to process movies' titles data.
2. The structure of the model used to process movies' posters are defined in the jupyter notebook file, using Tensorflow.Keras module.

## Project Outline
There are 4 main parts:
1. Preprocess Data: 
* Applying data preprocessing on movies' titles with Tokenization techniques
* Applying data preprocessing on movies' posters with Image Resizing, using OpenCV library.
2. Define Model:
* For movies' titles, the pre-trained BERT model is used.
* For movies' posters, the model structure is defined in the jupyter notebook file.
3. Train the models: Setting the Hyperparameters and using EarlyStopping
4. Evaluation: Using F1-score metric for overall evaluation

## Instructions to run the code:
In the "Movie_Genres_Classification.ipynb" jupyter notebook, select "Run all".
**Note:** There is a cell `!pip install -U transformers` in "Train the model for movies' titles" phase will require `Restart Session` so that you might have to select "Runtime" tab and "Restart Session and run all".