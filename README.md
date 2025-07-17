Melanoma type dectecor

This project uses the Jetson Orin Nano to analyze images and acuratly depict whether or not the image of melanoma entered is one of a benign tumor, or a malignant tumor.

![test](https://github.com/user-attachments/assets/82492cd9-a843-4fc5-8eb0-4d2c0e41bf47)
- this image depicts a malignant tumor that was accuatly classified by the software. 

How it works:
This algorithm works by useing the imagenet ai. Imagenet is a software that uses machine learning to disect data, find paternsbased off the data it was originally given. This is so when the user were to input an image, in this case an image of melanoma,the ai can accuratly give results about which class the image would fit into.

How to run the project:
1. To run the program, you first must download the project from github
2. Then open vs code and ensure you have python installed.
3. After that then you must open a new terminal
4. Set the NET and DATASET variables
   - NET=models/melanoma
   - DATASET=data/melanoma
6. Then run this command in the terminal: imagenet.py --model=$NET/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=$DATASET/labels.txt $DATASET/test/folder in which the image is stored/inputed image.jpg outputted image name.jpg
7. Then wait for the image to load

Heres a video link to the project!
https://youtu.be/Wtf9S7MIUIg

And heres a link to the dataset used in the project:
https://www.kaggle.com/datasets/dev523/leaf-disease-detection-dataset?select=dataset
