## Image Classification and Prediction with DINOv2 in Google Colab

`NOTE: This is validated in Google Colab T4 GPU`

Here we are going to discuss how to classify images using DINOv2 embeddings and a C-Support Vector Classification (SVC) linear classification model. We will have a model trained on the [Kaggle Vegiable Dataset](https://www.kaggle.com/datasets/misrakahmed/vegetable-image-dataset)  that classifies vegitable images.


### Clone DINOv2 install dependancies

#### Step 1

```
git clone https://github.com/facebookresearch/dinov2.git
```
#### Step 2
```
cd dinov2
```
#### Step 3
```
pip3 install -r requirements.txt

```

### For Download [Kaggle Vegiable Dataset](https://www.kaggle.com/datasets/misrakahmed/vegetable-image-dataset) follow below steps

#### Step1
```
pip3 install kaggle
```

#### Step 2
- Goto [Kaggle Settings](https://www.kaggle.com/settings)
- Click on `Create New Token` will get `kaggle.json` file 
- Put this json filr to `~/.kaggle/`

#### Step 3
Run following command that will download respecctive dataset 
```
kaggle datasets download -d misrakahmed/vegetable-image-dataset
```

### Execute Notebook
`dinov2_classify_and_predict.ipynb`

### Refference

1. https://github.com/facebookresearch/dinov2
2. https://www.kaggle.com/datasets/misrakahmed/vegetable-image-dataset
3. https://blog.roboflow.com/how-to-classify-images-with-dinov2/