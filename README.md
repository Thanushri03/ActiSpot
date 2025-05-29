# ActiSpot
An Intelligent System for Action Recognition and Localization
ActiSpot is an intelligent surveillance framework engineered to detect human actions in real-time video feeds by integrating advanced computer vision models—YOLOv8 for person detection and SlowFast for temporal action recognition.

The system first employs YOLOv8 to localize individuals in each frame, generating high-precision bounding boxes. These cropped regions are then passed through the SlowFast_64x2_R101_50_50 backbone pretrained on the AVA dataset, which specializes in learning multi-scale temporal features for nuanced action classification.

The model is capable of recognizing 80 atomic visual actions, including but not limited to sit, stand, walk, run, hug (a person), fight/hit (a person), cook, eat, drive, write, throw, watch (a person), and hand wave, among many others—thereby enabling the system to identify both physical behaviors and complex interactions with people or objects.

The pipeline is structured to deliver frame-level inferences with corresponding action labels and confidence scores, allowing for a comprehensive understanding of human activity within surveillance footage. Notably, the system achieves an impressive accuracy of 90%, underscoring its robustness and reliability in practical scenarios.

Designed for scalable deployment, ActiSpot is ideally suited for security analytics in public spaces, anomaly detection, and real-time behavioral intelligence across a wide spectrum of operational environments.
