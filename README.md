In this project, I present an end-to-end License Plate Recognition Pipeline utilizing deep learning and Optical Character Recognition (OCR) technology. The pipeline consists of six key steps, each contributing to the efficient and accurate recognition of license plates in images.

Step 1: Image Labeling
To kickstart the pipeline, I collect a dataset of images containing license plates. These images are then meticulously labeled using the Image Annotation Tool, an open-source Python GUI developed on GitHub. The labeling process prepares the data for training the deep learning object detection model.

Step 2: Training
With the labeled dataset in hand, I proceed to the data preprocessing stage. The preprocessed data is then used to train a sophisticated deep learning object detection model. For this project, I employ the powerful Inception ResNet V2 architecture in TensorFlow 2. This model is trained to accurately detect license plates in diverse images.

Step 3: Save Model
Once the training process is complete, I save the trained Inception ResNet V2 model. Saving the model enables me to use it for further tasks without the need for retraining, thus streamlining the pipeline's efficiency.

Step 4: OCR and Region of Interest (ROI) Extraction
The next step involves processing the images through the trained object detection model. The model identifies the license plate's region of interest (ROI) within each image. This ROI is then extracted for further analysis, isolating the license plate from the rest of the image.

Step 5: Optical Character Recognition (OCR)
The cropped license plate images are fed into the Tesseract OCR API, a powerful OCR engine developed in Python (PyTesseract). Tesseract effectively extracts the text content from the license plates, converting the visual information into readable text data.

Step 6: Building the Pipeline Deep Learning Model
Finally, armed with the OCR-extracted text and the corresponding cropped license plate images, I construct a cohesive Pipeline Deep Learning model. This model integrates the object detection and OCR functionalities into a single, robust system. The model can take any new image as input, proceed through the entire pipeline, and provide accurate recognition results for the license plate text.

<img width="524" alt="image" src="https://github.com/nehalsindhu12/license-plate/assets/111146044/6225d5b4-4556-4d1c-96e0-2bfaeffd6c2b">


