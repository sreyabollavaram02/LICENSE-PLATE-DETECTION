# LICENSE-PLATE-DETECTION
license plate  is extracted from image of a vehicle using Object detection and number is projected out using  Character recognition techniques.

# Introduction:

Automated license plate recognition systems employ image analysis to swiftly identify vehicles by their number plates, utilizing footage from video surveillance cameras. This advanced technology finds extensive utility in tasks such as toll collection, vehicle tracking, and the retrieval of stolen vehicles from CCTV records.

# Approach

In order to anticipate the license plate number :

1.  Initial detection of the license plate within the image frame was accomplished through  You-Only-Look-Once (YOLO v8) algorithm tailored to our specific requirements.
2.  Subsequently, the extracted license plate underwent a  process of character segmentation. This involved employing sophisticated techniques to identify and isolate individual characters, through the detection of rectangular contours, ensuring accurate representation of each character.
3.  The final critical phase involved character recognition, where we have implemented Convolutional Neural Networks (backpropagation method) . 

# Datasets:

1.	For license plate detection (YOLO): The dataset contains approximately 4000 annotated images of cars with license plates. The dataset can be found and downloaded from here https://data.mendeley.com/datasets/nx9xbs4rgx/2
2.	For character recognition:  We have created the dataset with about 400 images of digits from 0-9 and alphabets from A-Z .

# Method to execute :
if you want to train the entire model by yourself then you can first download both the datsets mentioned above and 1st open the license_plate_detection.ipynb file and change the paths to the dataset(license plate detection dataset) to where the dataset resides on your system and run the code step by step for license plate detection , and you can run the letter_recognition.ipynb file by changing the paths of dataset in code for  letter recognition.

If you want to use the pretrained weights you can download the folders detects(final weights  for plate detection stored in 25epoch_results/weights) and weights (contains final weights for letter_recognition)
and run final_LPD.ipynb file where we used the final weights, you can change the path to weights for both acoording to path of weights in your system to finally get an User interface  where you can directly upload photo to get license plate number 

# Performance Metrices

you can see all the performance metrices in detects folder(detects/25epoch_results) for performance evaluation on training data, (detects/val) stores the validation performance on testing data.






