# Motion Detection Using Python

This repository contains a Python program for motion detection using the OpenCV library. The program allows you to detect motion in a video stream or a webcam feed and highlight the areas where motion is detected. It also provides the option to save the output video with the motion highlights.

## Features

- Real-time motion detection: The program continuously analyzes the video frames and detects any motion occurring in the scene, providing instant feedback.
- Motion highlighting: Detected motion is visually highlighted in the video stream, making it easy to identify the areas where motion is occurring.
- Adjustable sensitivity: You can fine-tune the motion detection sensitivity by modifying the threshold value in the configuration file. This allows you to customize the detection algorithm to suit your specific needs.
- Configurable minimum area: The program allows you to set a minimum contour area threshold. Any detected motion with an area below this threshold will be disregarded. You can adjust this value based on your requirements.
- Gaussian blur for noise reduction: The frames are preprocessed with a Gaussian blur to reduce noise and enhance the accuracy of motion detection.
- Save output video: The program provides an option to save the processed video with the motion highlights as an output file. This allows you to review and analyze the detected motion later.
- Executable file provided: You can also run the motion detector using the provided executable file, making it easier to use the program without Python dependencies.

## Installation

1. Clone the repository to your local machine using the following command:

   ```
   git clone https://github.com/alok-2002/Motion_Detection_Using_Python.git
   ```

2. Navigate to the project directory:

   ```
   cd Motion_Detection_Using_Python
   ```

3. Install the required dependencies:

   ```
   pip install -r requirements.txt
   ```

## Usage

### Running with Python

To run the motion detection program using Python, use the following command:

```
python motion_detection.py
```

The program will open the webcam and start detecting motion. The areas where motion is detected will be highlighted in real-time. If you want to save the output video, press the 's' key.

Press the 'q' key to quit the program and stop the motion detection.

### Running with the Executable File

If you prefer not to run the program with Python, you can use the provided executable file. Simply double-click the `motion_detection.exe` file to start the motion detection program. The functionality and usage remain the same as running with Python.

Please note that the executable file is platform-specific, so make sure to use the appropriate file for your operating system.

## Configuration

You can modify the program's behavior by adjusting the configuration settings in the `config.json` file. The available configuration options are:

- `MIN_AREA`: The minimum contour area (in pixels) to be considered as motion. You can increase or decrease this value based on your needs.
- `THRESHOLD_SENSITIVITY`: The sensitivity of the motion detection algorithm. Higher values will detect smaller motion, while lower values may require larger motion to be detected.
- `BLUR_SIZE`: The size of the Gaussian blur kernel applied to the frames. Increasing this value can help reduce noise but may result in less precise motion detection.

## Contributing

Contributions to this repository are always welcome. If you find any issues or have suggestions for improvements, please create an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

This program is built using the OpenCV library. Special thanks to the developers of OpenCV for providing a powerful computer vision library that made this motion detection implementation possible.
