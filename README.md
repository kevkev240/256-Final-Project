# CSE256 Final Project: Cyberbullying Detection for Online Content

## Project Structure

### Directories
- **`data/`**  
  Contains raw and processed datasets used for the project. Not included in the repository due to large size. The data can be obtained online and preprocessed using the relavent notebooks.

  `messages.csv` contains the merges data with text and label, `train.csv` and `test.csv` are subset from train-test split.

  Raw dataset are from [Kaggle](https://www.kaggle.com/datasets/datadrivenx/cyberbullying-detection-dataset-for-online-content/data?select=1.+users_data.csv)

- **`model/`**  
  Stores Hugging Face's fine-tuned model's checkpoints. Not included in the repository due to size. Can be obtained using the code in `classification.ipynb`.

- **`results/`**  
  Directory for storing intermediate and final results.  
  - `fine_tuned_pred.json`: Predictions from the fine-tuned model.  
  - `pre_trained_pred.json`: Predictions from the pre-trained model.  
  - `perspective_pred.json`: Predictions using PerspectiveAPI.  
  - `perspective_probs.json`: Probability scores from PerspectiveAPI.  
  - `perspective_indices.json`: Indices corresponding to PerspectiveAPI results.

### Files
- **`data_processing.ipynb`**  
  Notebook for preprocessing the dataset, including merging and cleaning data.  

- **`data_exploration.ipynb`**  
  Notebook for exploring and analyzing the dataset (e.g., class distributions, message lengths).  

- **`classification.ipynb`**  
  Main notebook for data splitting, pretrained model fine-tuning, evaluation, and predictions using the DistilBERT model.

- **`perspective.ipynb`**  
  Notebook for making predictions using the PerspectiveAPI.

- **`analysis.ipynb`**  
  Notebook for performing error analysis of the models and trying ensembling techinques.

### Additional Information
This project utilizes various libaray and frameworks including Hugging Face Transformers, PyTorch, Scikit-Learn, etc.
