# DeepFake-Face-Detection

This project aims to uncover the distorted truth behind Deepfake media by building a system capable of identifying synthetic or manipulated visual content. Deepfakes are AI-generated media—usually videos or images—in which a person’s likeness is replaced or altered to make it appear that they said or did something they never actually did. Such content can be used maliciously to spread misinformation, defame individuals, or conduct fraud.

Objective: Detect and classify deepfake content to prevent its misuse in digital deception, misinformation campaigns, and online identity theft.
-------------------------------------------------------------------------------------------------------------------------------------------------------------
Preprocessing Techniques

To effectively train a deepfake detection model, the raw video or image data needs to be cleaned, standardized, and structured. This is done through several preprocessing steps, which ensure the model receives high-quality, consistent inputs.
1. Frame Extraction
What it is: Splitting video files into individual frames (images).
Why it’s important:
Models generally work on static images, so converting videos into frames provides many training samples.
Allows the model to analyze each frame independently for subtle inconsistencies that may indicate tampering.
Example: A 10-second video at 30 FPS yields 300 frames, all of which can be used as labeled data for training.
2. Facial Landmark Detection
What it is: Identifying and marking key facial points (eyes, nose, mouth, jawline) in each image or frame using computer vision algorithms.
Why it’s important:
Deepfakes often introduce small geometric or texture distortions around facial features.
Extracting the face region and aligning it based on landmarks improves the model’s ability to focus on critical areas.
It normalizes the orientation, size, and position of faces, making training data more consistent.
