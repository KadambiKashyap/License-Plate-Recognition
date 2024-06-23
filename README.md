# License Plate Recognition Project


### Problem Statement
Detecting and recognizing vehicle license plates represents a widely recognized challenge that has garnered significant attention. This challenge revolves around the utilization of two distinct datasets:

1. **Vehicle Images Dataset:** 900 images sourced from the internet and meticulously annotated with precise coordinates of bounding boxes encapsulating the license plates within each image.
2. **License Plate Images Dataset:** 900 images where the annotations take the form of the alphanumeric text inscribed on each license plate.

The primary aim of this task is twofold:
1. **Detection:** Identify and locate the license plates affixed to the vehicles in the images.
2. **Recognition:** Perform character recognition on these license plates, deciphering the alphanumeric text they contain.

### Dataset Organization
The dataset is organized into three distinct sets:
1. **Training Set 1:** 900 images featuring a single car along with its corresponding license plate. Annotations include the coordinates of the bounding box (ymin, xmin, ymax, xmax) that outlines the license plate in each image.
2. **Training Set 2:** 900 images focusing solely on license plates. Annotations contain the characters present on each license plate.
3. **Test Set:** 201 images, structured similarly to the first training set. The task is to detect the license plates within the images and recognize the characters on those plates.

### Evaluation Criteria
- **Pre-processing, data analysis, and understanding**
- **Data Exploration**
- **Model building**
- **Accuracy of the character recognition from the license plate**

## Installation

To install the necessary dependencies, run:

```bash
pip install -r requirements.txt
```

```bash
sudo apt-get install tesseract-ocr -y
sudo apt-get install tesseract-ocr-ara      # Install Arabic language pack
```

### Usage

1. **Pre-processing and Data Analysis**:
  - Load detection and recognition annotations from CSV files.
  - Visualize sample images and bounding boxes to understand the data distribution.
  
2. **Data Exploration**:
  - Explore datasets to gain insights into the data.
  - Check for any inconsistencies or missing values in the annotations.
  
3. **Model Building**:
  - Convert data to COCO format for training.
  - Use transformers and datasets to prepare the processor and model.
  - Train the model with the prepared datasets.
  - Use PyTesseract for building and training deep learning models.
  
4. **Evaluation**:
  - Evaluate the model's performance on test data.
  - Calculate and display the accuracy of the character recognition from the license plate.
