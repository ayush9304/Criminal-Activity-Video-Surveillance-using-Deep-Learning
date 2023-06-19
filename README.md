# Criminal Activity Video Surveillance using Deep Learning

Anomaly Recognition System, a real-time surveillance programme made to automatically detect and analyse signals of offensive or disruptive actions.

## Dataset
[UCF-Crime Dataset](https://webpages.charlotte.edu/cchen62/dataset.html)

## Architecture
#### Model Architecture
A video consists of an ordered sequence of frames. Each frame contains spatial information, and the sequence of those frames contains temporal information. To model both of these aspects, we use a hybrid architecture that consists of convolutions (for spatial processing) as well as recurrent layers (for temporal processing).

The first model i.e., CNN will be used to extract the (spatial) features and convert them into an encoded feature vector hence called an encoder. Similarly, the second model i.e., RNN will be used to process mini-batches of encoded frames to get the final classification result hence called a decoder.
![image](https://github.com/ayush9304/Criminal-Activity-Video-Surveillance-using-Deep-Learning/assets/56977388/c5567956-2665-4506-8d07-3dcfade40c99)

#### Video Processing Pipeline
For real-time video monitoring, an efficient video streaming pipeline is required to handle the video stream from CCTV in parallel to the inference of models using those frames and make the best use of available hardware resources to minimize latency. Hence in video streaming engine, we used multiprocessing to create two different parallel processes, one of them handles the video streaming from CCTV or any other video input device and the other process will handle the inference engine for parallel analyzing the video frames for classification.
![image](https://github.com/ayush9304/Criminal-Activity-Video-Surveillance-using-Deep-Learning/assets/56977388/1b6c5b5d-299b-4ff2-bbf6-5f76d37e8b76)

## Training
| ![image](https://github.com/ayush9304/Criminal-Activity-Video-Surveillance-using-Deep-Learning/assets/56977388/dbccd1de-0067-4930-86cd-0d3ea1cc648b) | ![image](https://github.com/ayush9304/Criminal-Activity-Video-Surveillance-using-Deep-Learning/assets/56977388/4512bff0-bdce-424f-afd5-8a566696de60) |
|------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------|

## Results
<img width="430" alt="image" src="https://github.com/ayush9304/Criminal-Activity-Video-Surveillance-using-Deep-Learning/assets/56977388/d23ec120-efc2-4aa0-a2e7-811fc231865f">
<img width="482" alt="image" src="https://github.com/ayush9304/Criminal-Activity-Video-Surveillance-using-Deep-Learning/assets/56977388/d0cc59ac-1b12-46d9-a7c8-367d4d7b24ad">
<img width="469" alt="image" src="https://github.com/ayush9304/Criminal-Activity-Video-Surveillance-using-Deep-Learning/assets/56977388/058b4c8f-2870-4e70-a3ba-64a20c944c63">
<img width="470" alt="image" src="https://github.com/ayush9304/Criminal-Activity-Video-Surveillance-using-Deep-Learning/assets/56977388/d7c74716-5b13-44f6-ae9c-ce1e4a204957">
