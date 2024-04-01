# neural-dart-vision
neural-dart-vision is a project aimed at developing a neural network-based solution for real-time detection of dart positions using images captured from a single camera. Implemented in C++, this project leverages the power of deep learning to accurately identify and track dart positions within the camera's field of view.

### Annotating Images for Model Training

When annotating images for training the neural network model, it's crucial to accurately label the portion of the dart tip that is stuck inside the dartboard or the entire tip. The annotated data serves as the ground truth for training the model to detect dart positions effectively.

**Annotation Tools:**

- **Bounding Box Annotation:** Use tools like LabelImg, VGG Image Annotator (VIA), or Labelme for annotating bounding boxes around the dart position.
  
- **Pixel-level Annotation:** For more precise annotation, consider tools like COCO Annotator or Labelbox, which allow for pixel-level segmentation annotation.

- **Personal Recommendation:** Personally, i highly recommend using a platform like roboflow.

**Example Annotation:**

Below is an example of how to annotate dart positions in an image using bounding boxes:

![Annotation Example](annotation_example.png)

In this example, the bounding box precisely outlines the area where the dart is stuck inside the dartboard.

**Note:** Ensure that annotated images are stored in a structured manner and are accompanied by corresponding annotation files containing information about the annotated regions.

By following these guidelines, you can create high-quality annotated datasets essential for training a robust neural network model for dart position detection.
