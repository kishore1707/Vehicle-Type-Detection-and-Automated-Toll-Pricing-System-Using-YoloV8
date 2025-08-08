# Vehicle-Type-Detection-and-Automated-Toll-Pricing-System-Using-YoloV8
This project presents an automated toll collection system that leverages the YOLOv8 deep learning model to detect different types of vehicles from a video feed. After identifying a       vehicle's class (e.g., car, bus, truck), the system automatically calculates and assigns the corresponding toll price, displaying it on the output video and generating real-time          revenue statistics.

📊 Dataset
  The model was trained on a custom dataset derived from the COCO dataset. The images were annotated and processed using Roboflow to create specific classes for this project: car, bus,     truck, and tempo traveller. The dataset was split into training and validation sets to ensure the model's accuracy and robustness.

🌟 Key Features
 * Real-time Vehicle Detection: Utilizes a fine-tuned YOLOv8 model for accurate and fast detection of multiple vehicle classes.
 * Automated Toll Calculation: Assigns a pre-defined toll price to each detected vehicle based on its class.
 * Annotated Video Output: Generates an output video with bounding boxes, vehicle class labels, and the calculated toll price overlaid on each frame.
 * Revenue Statistics: Calculates and displays the total number of vehicles detected and the total revenue collected.
 * Efficient Workflow: The entire process, from video input to statistical output, is streamlined for efficiency.
   
⚙️How It Works

  * The system follows a clear pipeline to achieve automated toll pricing:
  * Video Input: The system takes a video of road traffic as its primary input.
  * Frame-by-Frame Analysis: The video is broken down into individual frames for processing.
  * YOLOv8 Vehicle Detection: Each frame is passed through the fine-tuned YOLOv8 model, which identifies and classifies vehicles (bus, car, tempo traveller, truck) and draws bounding         boxes around them.
  * Toll Pricing: For each detected vehicle, the system looks up its class in a predefined dictionary to retrieve the correct toll price.
  * Output Generation: The model creates a new video file, annotating each frame with the vehicle's class and its toll price.
  * Statistical Reporting: Simultaneously, the system aggregates data on the number of vehicles and the total toll revenue, providing a summary at the end of the process.

🛠️ Technologies Used

 * Model: YOLOv8 (fine-tuned on a custom dataset)
 * Framework: Ultralytics
 * Dataset Annotation: Roboflow
 * Core Libraries: Python, OpenCV, PyTorch
   
▶️ Usage

 * Place your input video file (e.g., traffic.mp4) in the data/ folder.
 * Open the yolo_model_training.ipynb notebook.
 * Update the video input path in the prediction/inference cell to point to your video.
 * Run the cells in the notebook.
 * The output video and revenue statistics will be generated and saved.



