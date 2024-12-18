![Tracked with Occlusion Handling](assets/tracked_with_occlusion_handling.gif)


Video Tracking with Occlusion Handling
This script uses YOLOv8 for object detection and tracks items across video frames, handling temporary occlusions and organizing objects by shelves.

Features:
Object Tracking: Assigns unique IDs to detected objects and tracks them frame by frame.
Occlusion Handling: Retains object IDs when they temporarily disappear and reassigns them if they reappear.
Shelf Organization: Groups objects into shelves based on vertical alignment and labels them visually.
Lost Object Tracking: Displays IDs of objects that leave the scene.
Output Video: Saves a processed video with bounding boxes, shelf labels, and tracking details.


YOLOv8 Model Training
The YOLOv8 model used in this script is trained on the SKU110K dataset, a large-scale dataset of retail product images. The dataset is specifically designed for object detection tasks in cluttered environments, making it ideal for applications like shelf monitoring and inventory tracking.

Training Details:
Dataset: SKU110K, featuring over 11,000 images with densely packed objects.
Objective: Detect and localize small, densely arranged items typical of retail shelves.
Optimization: Fine-tuned to handle occlusions, varying object sizes, and complex backgrounds.
Output: A custom-trained YOLOv8 model optimized for high precision in structured environments.
This training ensures the model performs accurately in real-world scenarios like pharmacies and retail stores.


