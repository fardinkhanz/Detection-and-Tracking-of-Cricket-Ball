# Detection-and-Tracking-of-Cricket-Ball
![motivation2](https://github.com/fardinkhanz/Detection-and-Tracking-of-Cricket-Ball/assets/89691395/ca3491c2-bce4-40d7-9a4b-c8962477fadf)


This repository contains code and resources for the learning-based algorithm developed to detect and track balls in cricket videos. The algorithm combines the YOLOv7 model for ball detection and the BoT-SORT technique for ball tracking, resulting in improved speed, accuracy, and robustness compared to other real-time object detectors

## Features
* Utilizes the YOLOv7 model for ball detection, achieving superior performance in terms of both speed and accuracy.
* Outperforms other real-time object detectors with an accuracy of 56.8 percent AP at 30 FPS.
* Implements ball tracking using the BoT-SORT technique, incorporating motion and appearance data with camera-motion compensation and a more accurate Kalman filter state vector.
* Handles challenges such as the ball's constant movement, varying form and appearance, and frequent player occlusion.
* Determines the trajectory of the ball.
  ![yolo_bot_sort](https://github.com/fardinkhanz/Detection-and-Tracking-of-Cricket-Ball/assets/89691395/79a4eac7-7457-4bcd-8318-0dcdedd83b5e)


## Usage
* Prepare the cricket video file or stream that you want to analyze. Make sure the video is accessible and located in the appropriate directory.

* Run the main script, specifying the input video path, detection confidence threshold, and other parameters as required.
* The script will process the video, detect and track balls, and output the results.

## Contributing
Contributions to the project are welcome! If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request.

## Results 
In this chapter, the outcomes of several experiments conducted to improve object detection and tracking are discussed. The experiments were performed using the Yolo V7 model with varying epochs and datasets. 

Experiment 1 trained the model on a dataset consisting only of examples of balls. While the model successfully identified balls, it struggled to distinguish them from other objects.

Experiment 2 introduced a new class resembling a round ball (football) to address the limitations of the previous experiment. However, the model still had difficulty identifying balls when they were hazy or moving swiftly.

Experiment 3 increased the training dataset and applied random augmentations to improve ball detection in fuzzy images. This resulted in improved performance with higher mean average deep sort precision.

Experiment 4 incorporated a tracking algorithm using Yolo V7 deep sort, which plotted the ball's trajectory. However, the trajectory appeared scattered with low tracking accuracy.

In Experiment 5, the team addressed the issues from previous experiments by training the model on a dataset with separate classes for helmet, ball, and globe. They also utilized the bot-sort algorithm and data augmentation. This led to significant improvement in object detection and tracking accuracy, as demonstrated by the higher mean average precision and multiple object tracking accuracy. Visual results showed clearer and more accurate ball trajectories.
![experiment2output](https://github.com/fardinkhanz/Detection-and-Tracking-of-Cricket-Ball/assets/89691395/ba38637d-ca90-47d8-841e-0bd7bb22abb1)

## License
This project is licensed under the MIT License.

## References
* [1] BoT-SORT: Tracking by Detection for Real-Time Object Tracking. ([Link to paper](https://arxiv.org/abs/2206.14651))
* [5] You Only Look Once (YOLO): Unified, Real-Time Object Detection. ([Link to paper](https://arxiv.org/abs/2207.12202))
* Please cite the above references if you use this algorithm in your research or projects.

## Acknowledgements
We would like to acknowledge the contributions of the researchers and developers behind the YOLOv7 and BoT-SORT models, as well as the creators of the dataset used in this project. Their work has been instrumental in the success of this algorithm.
