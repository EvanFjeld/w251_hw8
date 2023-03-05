# w251_hw8

Using ffmpeg, i took a screenshot of the tesla cam every 5 seconds which left me with 152 images. I annotaded these images with 'car', 'truck', 'suv' using roboflow with their active learning feature to make the annotation go by significantly faster. There were too many pickup trucks in the images to not included that as a class. These broke down into 106 training images, 30 validation images, and 16 test images. The images for all three groupings and three classes can be found in the zip file in this git repo or in my public roboflow project here: https://app.roboflow.com/w251-8f2at/hw8-gnmlo/1


Trained for 10,000 steps and didn't quite cross .4 but got very close.

IoU metric: bbox
 Average Precision  (AP) @[ IoU=0.50:0.95 | area=   all | maxDets=100 ] = 0.335
 Average Precision  (AP) @[ IoU=0.50      | area=   all | maxDets=100 ] = 0.541
 Average Precision  (AP) @[ IoU=0.75      | area=   all | maxDets=100 ] = 0.351
 Average Precision  (AP) @[ IoU=0.50:0.95 | area= small | maxDets=100 ] = 0.194
 Average Precision  (AP) @[ IoU=0.50:0.95 | area=medium | maxDets=100 ] = 0.396
 Average Precision  (AP) @[ IoU=0.50:0.95 | area= large | maxDets=100 ] = 0.442
 Average Recall     (AR) @[ IoU=0.50:0.95 | area=   all | maxDets=  1 ] = 0.253
 Average Recall     (AR) @[ IoU=0.50:0.95 | area=   all | maxDets= 10 ] = 0.424
 Average Recall     (AR) @[ IoU=0.50:0.95 | area=   all | maxDets=100 ] = 0.424
 Average Recall     (AR) @[ IoU=0.50:0.95 | area= small | maxDets=100 ] = 0.239
 Average Recall     (AR) @[ IoU=0.50:0.95 | area=medium | maxDets=100 ] = 0.471
 Average Recall     (AR) @[ IoU=0.50:0.95 | area= large | maxDets=100 ] = 0.528

I tried to increase the number of steps but Google timed me out and let me know I would need to pay for more epocs. Given how close I was to .4, this isn't the time that I start paying for Google services. They make enough money without me. 
