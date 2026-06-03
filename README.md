\# Breadboard Object Detection CS470



This project uses computer vision and YOLOv11 object detection to identify components in breadboard circuit images. It was developed as part of a CS 470 machine learning project focused on supporting classroom STEM circuit activities.



\## Project Overview



The goal of this project is to detect important breadboard circuit components from an image before future pin mapping and circuit-correctness checking.



Detected classes:



\- Board

\- Light/Diode

\- Arduino

\- Resistor

\- Wire



\## My Contribution



My focus was Phase 3: object detection. I fine-tuned YOLOv11 models to detect breadboard components and evaluated the model using precision, recall, mAP metrics, confusion matrices, training curves, and qualitative prediction outputs.



\## Dataset and Model



The original dataset contained 46 labeled images. For the final version, the dataset was expanded to 106 labeled images. A Roboflow class-mapping issue was identified and corrected before retraining.



Models tested:



\- YOLO11n

\- YOLO11s

\- YOLO11m



The final model used YOLO11m trained on the corrected old + new dataset.



\## Final YOLO11m Results



| Metric | Score |

|---|---:|

| Precision | 96.8% |

| Recall | 97.4% |

| mAP50 | 98.0% |

| mAP50-95 | 78.4% |



\## Key Takeaways



The final model performed well at detecting major breadboard components. Wires remained the most difficult class because they are thin, curved, overlapping, and often partially hidden.



\## Technologies Used



\- Python

\- YOLOv11 / Ultralytics

\- Roboflow

\- Google Colab

\- PyTorch

\- OpenCV

\- Computer Vision

\- Object Detection



\## Note



This is a class project prototype. The detector works well on the current dataset but would need more varied images and additional testing before real classroom deployment.



