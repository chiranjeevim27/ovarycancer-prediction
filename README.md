# Ovarian Cancer Detection using Transfer Learning

This repository contains code for detecting ovarian cancer using deep learning and transfer learning techniques. The project utilizes the DenseNet169 architecture pretrained on ImageNet and fine-tuned on a dataset of ovarian cancer images.

## Dataset

The dataset used for this project is the [Ovarian Cancer dataset](https://www.kaggle.com/datasets/rdhenkawat/ovarian-cancer) available on Kaggle. It consists of images related to ovarian cancer.

## Data Preprocessing

The dataset undergoes preprocessing, including resizing all images to 128x128 pixels and data augmentation using the Keras ImageDataGenerator.

## Model Architecture

The project employs transfer learning with the [DenseNet169](https://keras.io/api/applications/densenet/) architecture, pretrained on ImageNet. The final layers are modified for binary classification, distinguishing between cancerous and non-cancerous images.

## Training

Training is performed using an ImageDataGenerator for both training and validation sets. The model is trained for multiple epochs with callbacks for model checkpointing, learning rate reduction, and early stopping.

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/chiranjeevim27/ovarycancer-prediction.git
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Download the dataset from the provided Kaggle link and place it in the `/content/train1` directory.

4. Run the Jupyter Notebook:

   ```bash
   jupyter notebook ovary.ipynb
   ```

## Files

- `ovary.ipynb`: Jupyter Notebook containing the entire code for the ovarian cancer detection.
- `requirements.txt`: File listing the required Python dependencies.

## Results

The trained model achieves a certain level of accuracy in detecting ovarian cancer. Check the model performance and accuracy in the training history.

## Contributors

- Chiranjeevi M (https://github.com/chiranjeevim27/)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

Feel free to contribute, report issues, or suggest improvements!
