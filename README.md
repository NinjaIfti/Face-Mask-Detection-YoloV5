
**

 - [ ] 

# Face Mask Detection with YOLOv5

**
**A deep learning-based solution for detecting face masks in images and live video feeds using the YOLOv5 framework. This project helps ensure safety by identifying people with and without masks in real-time.**

***

## *Features*

***

 - Detects faces with and without masks in images, videos, and live
   streams.
   
  
 - High accuracy and fast inference speed using YOLOv5.
 - Supports both CPU and GPU for inference. 
 - Customizable confidence threshold and input sizes.

## ***Installation***

***Prerequisites***

 - [ ] Python 3.7 or higher
 - [ ] PyTorch installed (with GPU support if available)
 - [ ] pip package manager

**Steps**

 - [ ] Clone the Repository

        git clone https://github.com/NinjaIfti/Face-Mask-Detection-YoloV5.git
       cd face-mask-detection

**Set up a Virtual Environment (Optional but Recommended) A virtual    environment helps isolate project dependencies, making it easier    to manage and avoid conflicts with other Python projects on your    system.**

       
   

 - [ ] Create a Virtual Environment:

        python -m venv yolov5-env
        Activate the Virtual Environment:

On Linux/macOS:

    
    source yolov5-env/bin/activate
    
On Windows:

    yolov5-env\Scripts\activate
   

 - [ ] Install Dependencies Once the virtual environment is active,
       **install the required dependencies:**
       
        pip install -r requirements.txt
 - [ ] Download Pre-trained YOLOv5 Model You can either use a
       pre-trained YOLOv5 model or train a custom model for face mask
       detection.

**To use the pre-trained model, simply download it:**

     wget https://github.com/ultralytics/yolov5/releases/download/v5.0/yolov5s.pt

 - [ ] Running the Detection

**On Images**

    bash
    python detect.py --source images --weights yolov5s.pt --conf 0.5

**On Video**

    bash
    python detect.py --source video.mp4 --weights yolov5s.pt --conf 0.5

**The detected results will be saved in the runs/detect/exp folder.**

**Live Detection**
For live webcam detection, simply run:

    bash
    python detect.py --source 0 --weights yolov5s.pt --conf 0.5

*

# ***How It Works***

*

**Model Training**

The model is based on YOLOv5, a state-of-the-art object detection model. It has been fine-tuned to detect faces and classify them as "with mask" or "no mask."

**Image and Video Processing**

Once the model is loaded, it takes images or video frames as input, performs face detection, and classifies the face as either "mask" or "no mask."

*

# ***Troubleshooting***

*

**Error: ModuleNotFoundError**

If you encounter errors related to missing modules, ensure that all dependencies are installed using:

    bash
    pip install -r requirements.txt


**Low Detection Accuracy**

If the model doesn't perform well, consider retraining it with your own dataset for better accuracy.

**License**

This project is licensed under the MIT License - see the LICENSE file for details.


*

## *****Acknowledgments*****

*

## YOLOv5

## OpenCV

## PyTorch


