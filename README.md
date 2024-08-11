Weapon detection is a critical facet of security and surveillance technology, involving the 
automated identification and localization of firearms, explosives, or other hazardous objects 
within visual data such as images or videos. Employing advanced technologies like computer 
vision and deep learning, weapon detection systems leverage models such as Convolutional 
Neural Networks (CNNs) to recognize intricate patterns and features associated with weapons. 
Commonly applied in security screening at airports, public events, and high-security facilities, 
as well as in surveillance systems and law enforcement, weapon detection contributes to swift 
responses to potential threats.

The core of the system is the YOLOv8 model itself. This pre-trained model, 
specifically designed for weapon detection, analyses each frame. It predicts bounding 
boxes around detected objects and assigns confidence scores indicating the likelihood 
of a weapon being present. 
Following this, there can be a post-processing stage. Here, low-confidence detections 
are filtered out to minimize false alarms. Additionally, techniques like Non-Maxima 
Suppression can be used to refine overlapping bounding boxes. Optionally, object 
tracking can be implemented to follow the movement of detected weapons across 
video frames. 

![image](https://github.com/user-attachments/assets/bc472840-1813-4626-b971-e5a689bd8511)


After successfully training our custom YOLOv8 weapon detection model, we 
expanded its utility by developing a robust API (Application Programming Interface). 
This API serves as a standardized interface for seamless integration of our model into 
various applications and services. Leveraging Flask, a lightweight web framework for 
Python, we meticulously crafted RESTful API endpoints that facilitate both real-time 
and batch processing of weapon detection tasks. The API allows clients to send image 
data to the server, where the YOLOv8 model performs inference and returns results, 
maintaining a scalable and efficient communication protocol.
