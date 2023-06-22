# Defect Detection in Wood Surfaces
## Project Description
This project aims to develop and evaluate a model that detects defects in wood surface images. The data for this project was collected from multiple locations and the model is primarily developed for a specific location, Location 3.

In the dataset, there are 11 unique labels. Label 0 represents "no defect", while labels 1-10 represent specific types of defects. Images may contain combinations of these labels.

## Data
You can find the dataset:

- train_input: RGB images of wood boards from various locations.
- train_labels: Segmentation masks of wood boards. (Values are the labels 0-10, refrain from using a greyscale encoding for plotting the masks)
- train_defect_information: A CSV file which contains filenames and the occurrence of a specific label as a boolean.
CSV Content
- img_filename: filename of train_input
- mask_filename: filename of train_labels
- location: Location of data collection
- contains_label_x (x: 0 - 10): Occurrence of specific label in the image
- test_input: RGB images of wood boards exclusively from Location 3