# Document-Scanner

This project can be used for scanning handwritten notes and print documents. This project will scan a document with the help of webcam, then it will print the scanned document which is stacked with original document.

This is the primary project in OpenCV, which uses **first priciples of Computer Vision**. 

It automatically detect the edge of the paper over a contrasting surface. When using the printed special page template it automatically detects the QR Code printed on the bottom right corner and scans the page immediately. After the page is detected, it compensates any perspective from the image adjusting it to a 90 degree top view and saves it on a folder on the device.

It also incorporates OCR functionality which the user can use to detect text from documents and save them as editable text files in the external storage of the device.

# Pipeline of the project

- First, it will get the original documnet image from the webcam
- It will convert this image into grayscale image
- Apply Edge detector to find edges
- Find counters all the contours present in the image
- From this we filter, and find the biggest contour
- With the corner of the biggest contour, we will use Warp Prespective to get the desired image
- Later, we will apply adaptive thresholding to get the scanned paper feel
- lastly, we will save this scanned image into a folder
- 

# Technologies
- OpenCV
- Python

# Features
- Scan handwritten or printed documents
- Detects page frame and corrects perspective
- Fast and smooth Image Processing on the fly
- Scans are saved to your device as images
- Detect text using the OCR functionality of the app
- Save the detected texts as editable text files to your device.
- Easily share scanned docs with others via social media, email attachment or sending the doc link.
