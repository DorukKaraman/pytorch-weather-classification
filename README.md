# PyTorch Weather Classification

This project builds and compares three different neural network models to classify weather images into four categories: **Cloudy**, **Rain**, **Shine**, and **Sunrise**. ☀️🌧️☁️🌅

The models implemented are:
1.  A simple **Fully-Connected Network (FCN)**
2.  A custom **Convolutional Neural Network (CNN)**
3.  A **Transfer Learning** model using a pre-trained **ResNet-18**

This project is a refactored and cleaned-up version of a university assignment, intended as a portfolio project to demonstrate data loading, model building, training, and evaluation in PyTorch.

## Models & Results

Here are the performance metrics achieved on the **test set**:

| Model                 | Test Accuracy | Test Precision (Macro) | Test Recall (Macro) | Test F1 (Macro) |
| :-------------------- | :-----------: | :--------------------: | :-----------------: | :-------------: |
| **FCN** |   ~78.7%      |        ~78.8%          |       ~77.0%        |     ~77.6%      |
| **CNN** |   ~79.1%      |        ~82.1%          |       ~80.0%        |     ~76.4%      |
| **ResNet-18 (Transfer)** |   ~96.9%      |        ~97.0%          |       ~96.6%        |     ~96.8%      |

*(Note: The ResNet-18 Transfer Learning model significantly outperforms the custom FCN and CNN models, demonstrating the effectiveness of leveraging pre-trained weights.)*

## Dataset

This project uses the **Multi-class Weather Dataset for Image Classification**, example is provided. 


## How to Use

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/DorukKaraman/pytorch-weather-classification.git](https://github.com/DorukKaraman/pytorch-weather-classification.git)
    cd pytorch-weather-classification
    ```

2.  **Install Dependencies:**
    The project requires the following Python libraries:
    * `pytorch` (`torch`)
    * `torchvision`
    * `numpy`
    * `matplotlib`
    * `scikit-learn`
    * `seaborn`
    * `pillow` (PIL)
    * `tqdm`

    You can install them using pip:
    ```bash
    pip install torch torchvision numpy matplotlib scikit-learn seaborn pillow tqdm
    ```

3.  **Set up the Data:**
    * Ensure the directory structure looks like this:

        ```
        pytorch-weather-classification/
        ├── Weather_Classification.ipynb
        ├── data/
        │   └── Multi-class Weather Dataset/
        │       ├── Cloudy/
        │       │   ├── ... (images)
        │       ├── Rain/
        │       │   ├── ... (images)
        │       ├── Shine/
        │       │   ├── ... (images)
        │       └── Sunrise/
        │           ├── ... (images)
        └── README.md
        ```

4.  **Run the Notebook:**
    Open and run the `Weather_Classification.ipynb` notebook using Jupyter Lab or Jupyter Notebook. Make sure the `DATA_DIR` variable points to the correct dataset location.
