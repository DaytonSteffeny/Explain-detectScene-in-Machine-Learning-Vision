# Explain Detect Scene in Machine Learning Vision


## About the project:
This app uses different functions to detect what the image is. It anyalizes the image using the function **detectScene(image: CIIamge)** which displays the percentage of what image (type CIImage) might be. It uses function **photoLibraryselected** to pick an image to upload.

This app uses two different functions to grab results for the image and importing to the UI. It also uses an IBOutlet **activityIndicator: UIActivityIndicatorView!**. The function didRecieveMemoryWarning is a warning if it did or did not recieve memory error. The iboutlet **cameraSelected** enables the user to be able to take a photo and upload it the app. If it recieve the error it sends a message, if not then it will upload. The function **imagePickerController** uploads the selected image to the app to be used in the dectectScene function.
The dectectScene function  will load the ML model through its generated class. If the ML model cannot load, display a message and return value.
The last function is to run the Core ML GoogleNetPLaces classifier to ciImage to dectect the image and to give a percentage of what it might be.
