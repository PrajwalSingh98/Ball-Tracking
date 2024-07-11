# Ball-Tracking
The task assigned was to create a computer vision program to track the movement of balls of different colors across various quadrants in a provided video. The program was expected to record events of each ball entering and exiting each numbered quadrant in the format: ***Time, Quadrant Number, Ball Colour, Type (Entry or Exit)***. The processed video would display ball tracking with color, overlay text indicating "Entry" or "Exit" along with a timestamp, and generate a text file recording these events.

## Achievements
* **Ball Detection:** Successfully detected all balls except the golf ball.
* **Tracking and Event Recording:** Implemented the functionality to track the movement of balls and record events in the specified format.
* **Processed Video:** Created a processed video with overlays indicating ball movement events and timestamps.

## Challenges and Limitations
* **Golf Ball Detection:** The golf ball posed a significant challenge due to its white color, which blended with the background. Efforts to create a color mask for detection were unsuccessful due to the lack of contrast and the ball's lack of smooth edges, complicating edge detection methods.

* **Peach Ball Detection in Second Quadrant:** The peach-colored ball was inconsistently detected in the second quadrant, likely due to variations in lighting conditions or inaccuracies in defining the color range for peach. Further refinement of the color range or additional preprocessing steps might be needed to enhance detection accuracy.

* **Occlusion Handling:** The program faced difficulties when the ball was temporarily obscured by a hand. When the ball became visible again, it was erroneously recorded as a new entry event, despite not having moved from its place. This issue arises from the inability of the current model to account for temporary occlusions without reinitializing the detection.

## Conclusion

While the program achieved the primary objectives of detecting and tracking multiple colored balls and recording their movements across quadrants, certain limitations affected the accuracy and reliability of the results. In particular, the detection of the white golf ball and handling of occlusions require further refinement. Despite these challenges, the core functionalities were implemented successfully, and the program produced meaningful outputs as specified.
