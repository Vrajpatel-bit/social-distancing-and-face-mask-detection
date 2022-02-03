# social-distancing-and-face-mask-detection

According to data obtained by the World Health Organization, the global pandemic of COVID-19 has severely impacted the world and has now infected more than fifteen
crore people worldwide. Wearing face masks and following
safe social distancing are two of the enhanced safety protocols that need to be followed in public places in order to
prevent the spread of the virus. To create a safe environment that contributes to public safety, we have implemented
an efficient, lightweight and robust computer vision based
approach focused on the real-time automated monitoring of
people to detect both safe social distancing norms and face
masks detection in public places. In this proposed system
we are using modern deep learning algorithms, OpenCV
and Tensor flow for pre-processing, objection detecting and
calculating the distance between people with the help of
distance based methods. Due to the lack of labelled video
dataset in the community we have used two video dataset
taken from Youtube. Also the average prediction time is kept
as fast as possible, for a generated video of 50 seconds with
a fps of 25, the average time for each frame is 4.5 seconds.
Thus, the proposed system favors the society by saving time
and helps in lowering the spread of coronavirus. It can be
implemented effectively in the current situation when lockdown is eased to inspect people in public gatherings, shopping malls, public streets, work places, etc. Automated inspection reduces manpower to inspect the public and also
can be used in any place.

This provides a deep learning model which can help to classify between masked and
unmasked people. And also find the number of people at
risk who are violating social distancing.

The method for the face mask classification takes the
video or image as an input. The preprocessing is done on
the Image and each video frame. Using the deep learning model, the face mask classification is done and shows
the results. For this project we attempted to create a Computer Vision software that can detect a face mask on a live
video feed using a lightweight Convolutional Neural Network (CNN), MobileNetV2 built on top of TensorFlow machine learning platform. The objective is to implement this
solution without using any expensive hardware so that it can
be used and run by students on a low budget.

For detecting social distancing in each video frame, we have
used YOLOv3 that is pre-trained on COCO’s dataset. The
COCO dataset has many classes out of which we are interested in the person class. As the model is pre-trained,
there is no need to train it again. In each frame YOLOv3
extracts the ROI of the people class and a bounding box is
generated. Non-maximum suppression is used to remove
the redundant and unnecessary bounding boxes from each
detected person.

After testing the model with different scenarios and different model configurations, the face mask model achieved
a training accuracy of 99.8% and testing accuracy of 99.5%.
Refer to figure 4 for the MobilnetV2 performance graph.
For the social distancing, after experimenting with different
values for non-maximum suppression 0.5 NMS threshold
showed the best results. For the distance metric, different
distance metrics were tried like Euclidean Distance, Manhattan Distance, etc. Finally, the Euclidean distance was
used to calculate the distance between each pair of people
in the frame. We have kept 100 pixels as the minimum distance. With all the above configurations, the social distancing model gave good results. 
