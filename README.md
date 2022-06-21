# wce
introduction and modules 
  
	Object Detection Model    
In this study, Caffe deep learning model framework is used to run the object detection model. The model chosen is MobileNet SSD due to the short time taken for the execution.
SSD MobileNet obtained the best detection rate of 87.7% with a ratio of training to test data of 80:20 [11].

	Determine person location
In determining the position of a person’s bounding box as well as the segment involved, each ground plane point is used to compare the ROI range.  Surveillance cameras are usually placed at high places as the overhead camera specially to monitor a certain area e.g., high-risk area or areas of interest for an organization. In this case, it is more suitable to compare the ground plane for the detection box instead of using the center point value.

	Calculate the center point in the bounding box
To measure the center point, C (x, y) of the bounding box for the detected person, a midpoint equation is used a
                

Each of the minimum and maximum values for the corresponding width, xmin+xmax and height ymax+ymin, of the bounding box will be used to calculate the center point of the bounding box.

	Calculate distance between bounding box
To measure the distance, c(xmin,ymin)\ and\ c(xmax\ ,ymax)\ between each of the detected persons in the frame, distance equation is used as in (2).

D=√ (xmax-xmin)²+( ymax-ymin)²)        

the center point of the bounding boxes is taken to determine between two different locations of the bounding boxes. After getting the center points value, the algorithm will calculate if the distance is lower or higher than 2metres or the converted pixels.

implementation
step-1: Download and install Annaconda Software.

Step-2: Open Annaconda prompt.

Step-3: Install Opencv and Imutils libraries in annaconda propmpti.e. pip install opencv-python
     pip install imutils   
Step-4: Save the social-distancing-detector Folder

Step-5: Reach the directory of person_detector.py in Annaconda prompt

Step-6: Execute the person_detector.py file in Annaconda prompt.
(NOTE:  The testvedio2.mp4  is inside the social distancing zip  file)
Example 
 ![image](https://user-images.githubusercontent.com/89571994/161952556-fc9364d4-8ced-4ab9-a4e2-85a70140f5e0.png)

