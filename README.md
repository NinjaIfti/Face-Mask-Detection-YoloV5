<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Face Mask Detection Using PyTorch</title>
</head>
<body>
    <h1>Face Mask Detection Using PyTorch</h1>
    <p>
        This repository contains a face mask detection system implemented using PyTorch. 
        The model is capable of detecting whether a person is wearing a mask or not in images, videos, and live webcam feeds.
    </p>

    <h2>Features</h2>
    <ul>
        <li>Mask detection in static images.</li>
        <li>Real-time detection via webcam.</li>
        <li>Easy-to-train custom models with PyTorch.</li>
        <li>Supports custom datasets for retraining.</li>
    </ul>

    <h2>Installation</h2>
    <ol>
        <li>Clone this repository:
            <pre><code>git clone https://github.com/yourusername/face-mask-detection</code></pre>
        </li>
        <li>Navigate to the project directory:
            <pre><code>cd face-mask-detection</code></pre>
        </li>
        <li>Install the required dependencies:
            <pre><code>pip install -r requirements.txt</code></pre>
        </li>
    </ol>

    <h2>Usage</h2>
    <h3>Detecting Masks in Images</h3>
    <p>To run detection on images, use the following command:</p>
    <pre><code>python detect.py --source Images --weights best.pt --conf 0.5</code></pre>

    <h3>Detecting Masks in Video Files</h3>
    <p>For video file detection:</p>
    <pre><code>python detect.py --source path_to_video.mp4 --weights best.pt --conf 0.5</code></pre>

    <h3>Live Webcam Detection</h3>
    <p>To use a webcam feed:</p>
    <pre><code>python detect.py --source 0 --weights best.pt --conf 0.5</code></pre>

    <h2>Training the Model</h2>
    <p>You can train the model using your own dataset:</p>
    <ol>
        <li>Organize your dataset with images and corresponding labels.</li>
        <li>Modify the <code>data.yaml</code> file to reflect your dataset structure.</li>
        <li>Run the training script:
            <pre><code>python train.py --data data.yaml --weights yolov5s.pt --epochs 50</code></pre>
        </li>
    </ol>

    <h2>Results</h2>
    <p>Sample output images with detections:</p>
    <ul>
        <li><strong>Mask Detected:</strong></li>
        <img src="results/mask_example.jpg" alt="Mask Example" width="300">

        <li><strong>No Mask Detected:</strong></li>
        <img src="results/no_mask_example.jpg" alt="No Mask Example" width="300">
    </ul>

    <h2>Supported Models</h2>
    <p>This project supports multiple models, including:</p>
    <ul>
        <li>YOLOv5</li>
        <li>RetinaFace</li>
        <li>Custom PyTorch-based models</li>
    </ul>

    <h2>Contributing</h2>
    <p>
        Contributions are welcome! Feel free to open issues or submit pull requests to improve the project.
    </p>

    <h2>License</h2>
    <p>This project is licensed under the MIT License.</p>

    <h2>Acknowledgments</h2>
    <ul>
        <li><a href="https://pytorch.org/">PyTorch</a></li>
        <li><a href="https://github.com/ultralytics/yolov5">YOLOv5</a></li>
        <li><a href="https://github.com/biubug6/Pytorch_Retinaface">RetinaFace</a></li>
    </ul>
</body>
</html>
