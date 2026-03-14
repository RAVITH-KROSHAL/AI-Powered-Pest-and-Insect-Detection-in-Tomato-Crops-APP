# AI-Powered-Pest-and-Insect-Detection-in-Tomato-Crops-APP

This project presents an AI-powered pest and insect detection system for tomato crops using deep learning and computer vision techniques. The system is designed to assist farmers in identifying harmful pests at an early stage, enabling timely intervention and reducing crop damage.

Early pest detection plays a crucial role in improving tomato yield and supporting sustainable agricultural practices. Traditional manual inspection methods are time-consuming and often inaccurate. This project introduces an automated detection framework that leverages the YOLOv8 object detection model to identify pests and insects in tomato plants in real time.

The model was trained on a hybrid dataset consisting of images collected from public datasets and real-world tomato farms, allowing the system to perform reliably under diverse environmental conditions.


* Key Features

1. Real-time pest and insect detection

2. AI-powered object detection using YOLOv8

3. Supports precision agriculture and smart farming

4. Multi-class detection for tomato pests and plant parts

5. Capable of detecting pests under different lighting and field conditions


* Dataset

The dataset used in this project is a hybrid dataset created from multiple sources:

1. Kaggle Tomato Pest Dataset

2. Roboflow Annotated Tomato Insect Dataset

3. Self-captured field images from tomato farms in Sri Lanka


* Detected Classes (12)

1. Caterpillars

2. Fruit Borers

3. Aphids

4. Whiteflies

5. Spider Mites

6. Thrips

7. Leaf Miners

8. Mealybugs

9. Pest Damage

10. Healthy Tomato Leaf

11. Healthy Tomato Fruit

12. Tomato Flowers

Images were resized to 640×640 pixels and augmented using rotation, flipping, mosaic augmentation, brightness/contrast adjustments, and color jittering to improve model generalization.


* Model Architecture

This project uses YOLOv8 (You Only Look Once version 8) for object detection.


Parameter	         Value
1. Model	          YOLOv8n
2. Input Size	      640×640
3. Epochs	          100
4. Batch Size     	16
5. Optimizer       	SGD
6. Learning Rate  	0.001

Training was conducted using Google Colab Pro with NVIDIA Tesla T4 GPU, while data annotation and preprocessing were performed using Roboflow.

Model      Performance
1. Metric	      Value
2. Precision   	74.7%
3. Recall	      68.3%
4. mAP@50	      73.3%
5. mAP@50–95	    41.4%


The system achieved real-time inference speed above 30 FPS, making it suitable for integration with mobile devices or drones for field monitoring.


* Technologies Used

1. Python

2. YOLOv8 (Ultralytics)

3. OpenCV

4. Roboflow

5. Google Colab

6. Deep Learning & Computer Vision


* Applications

1. Smart agriculture

2. Automated pest monitoring

3. Precision farming systems

4. Drone-based crop inspection


* Future Improvements

1. Integration with mobile applications for farmers

2. Deployment on edge devices (NVIDIA Jetson Nano)

3. IoT-based camera monitoring systems

4. Cloud dashboard for real-time pest alerts


Author

Ravith Kroshal Herath,
Faculty of Computing,
Sri Lanka Institute of Information Technology (SLIIT)
