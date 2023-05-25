# Human-speed-detection



This Python script detects and tracks faces in a video and calculates their speeds. It utilizes the OpenCV library for video processing and face detection. The script employs the Manhattan distance formula to estimate the speed of the tracked faces.

## Introduction

The script takes a video file as input and analyzes each frame to detect faces using the Haar cascade classifier provided by OpenCV. It maintains a list of centroids representing the faces' positions in consecutive frames. By comparing the centroids' positions, it determines whether a face in the current frame corresponds to a face in the previous frame.

## Calculation of Speed

Once a face is successfully tracked, the script calculates its speed by measuring the displacement between consecutive frames. It utilizes the Manhattan distance between the centroids of the corresponding rectangles in the frames. The distance is divided by a scaling factor (0.25) to estimate the face's speed.

## Usage

To use the script, follow these steps:

1. Make sure you have the required libraries installed: OpenCV, NumPy, and Matplotlib.
2. Clone the repository or download the script file.
3. Ensure the video file you want to analyze and the `frontalface.xml` file are in the same directory as the script.
4. Open a terminal or command prompt and navigate to the directory containing the script.
5. Run the script using the following command:
     
     `python speed.py` 


6. Enter the name of the input video when prompted. If you want to use the webcam as the input source, enter `0`.
7. Choose whether to suppress the streaming of the output video (`y` for yes, `n` for no).
8. Optionally, select whether to generate graphs based on the input video (`y` for yes, `n` for no).
9. The processed video will be saved as `processed-[filename].avi` in the current directory.
10. If you choose to generate graphs, they will be saved in an `output-[filename]` directory.
11. You can find a copy of the processed video on your desktop.

Please note that the script requires the `frontalface.xml` file, which is a pre-trained classifier for face detection. Ensure that it is present in the same directory as the script.

## Final Output would look like below Image





![image](https://github.com/Shivam7-1/Human-speed-detection/assets/55046031/02a039ba-fc4b-48b2-b087-a0d437028394)
