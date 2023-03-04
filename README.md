# w251_hw8

Using ffmpeg, i took a screenshot of the tesla cam every 5 seconds which left me with 152 images. I annotaded these images with 'car', 'truck', 'suv' using roboflow with their active learning feature to make the annotation go by significantly faster. There were too many pickup trucks in the images to not included that as a class. These broke down into 106 training images, 30 validation images, and 16 test images. The images for all three groupings and three classes can be found in the zip file in this git repo or in my public roboflow project here: https://app.roboflow.com/w251-8f2at/hw8-gnmlo/1




Train for as many epochs as needed to cross the 0.4 IoU=0.50:0.95
