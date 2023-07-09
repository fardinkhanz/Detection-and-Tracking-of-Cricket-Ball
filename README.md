# Detection-and-Tracking-of-Cricket-Ball
This repository contains code and resources for the learning-based algorithm developed to detect and track balls in cricket videos. The algorithm combines the YOLOv7 model for ball detection and the BoT-SORT technique for ball tracking, resulting in improved speed, accuracy, and robustness compared to other real-time object detectors

## Features
* Utilizes the YOLOv7 model for ball detection, achieving superior performance in terms of both speed and accuracy.
* Outperforms other real-time object detectors with an accuracy of 56.8 percent AP at 30 FPS.
* Implements ball tracking using the BoT-SORT technique, incorporating motion and appearance data with camera-motion compensation and a more accurate Kalman filter state vector.
* Handles challenges such as the ball's constant movement, varying form and appearance, and frequent player occlusion.
* Determines the trajectory of the ball.

## Usage
* Prepare the cricket video file or stream that you want to analyze. Make sure the video is accessible and located in the appropriate directory.

* Run the main script, specifying the input video path, detection confidence threshold, and other parameters as required.
* The script will process the video, detect and track balls, and output the results.

## Contributing
Contributions to the project are welcome! If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License
This project is licensed under the MIT License.

## References
* [1] BoT-SORT: Tracking by Detection for Real-Time Object Tracking. ([Link to paper](https://arxiv.org/abs/2206.14651))
* [5] You Only Look Once (YOLO): Unified, Real-Time Object Detection. ([Link to paper](https://arxiv.org/abs/2207.12202))
* Please cite the above references if you use this algorithm in your research or projects.

## Acknowledgements
We would like to acknowledge the contributions of the researchers and developers behind the YOLOv7 and BoT-SORT models, as well as the creators of the dataset used in this project. Their work has been instrumental in the success of this algorithm.
