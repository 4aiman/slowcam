# SlowCam

SlowCam is **a virtual green backdrop**. It basically replaces every thing around you by green color. So that you can use the Chroma Key filter in OBS Studio to put yourself in any other video. 
SlowCam is powered by a machine learning technology called [Tensorflow](https://github.com/tensorflow/tfjs) and its public model [BodyPix](https://github.com/tensorflow/tfjs-models/tree/master/body-pix).

I was unable to make it work fast enough with any amount of tweaking on Ryzen 5 3600 + RTX4070.
Maybe with a different model it'll work faster.

| | |
|----|----|
|Pros|Utilizes GPU unlike many alternatives|
|Cons| slow, hogs GPU and CPU resources|

Temp graphs<br>
![image](https://github.com/4aiman/slowcam/assets/2913210/35471699-5c6a-4b69-b327-62241a3bf187)<br>
![image](https://github.com/4aiman/slowcam/assets/2913210/b83b87a8-633a-4a65-ae4d-f90da770778f) CPU temp 
![image](https://github.com/4aiman/slowcam/assets/2913210/49459b33-39e5-4cd5-943b-90bf9c9fb284) NVME temp
![image](https://github.com/4aiman/slowcam/assets/2913210/3dd7c915-1d9a-4a56-82e1-c51c2442deae) RTX 4070 temp


GPU utilization alone:<br>
![image](https://github.com/4aiman/slowcam/assets/2913210/1824eb17-8e4b-48bd-a9e8-f89a0a54009e)


## How to use

### Follow steps below to setup:
Before you start: [![Check this](https://api.netlify.com/api/v1/badges/4ccf5f3b-b414-4da1-bf50-97955adbd300/deploy-status)](https://greencam.netlify.app) will show you how even with RTX4070 it's lagging like hell

Install locally if it somehow runs fine for you:
```
$ npm install
```
I had node v21, so this popped out:<br>
![image](https://github.com/4aiman/slowcam/assets/2913210/af6a234b-1010-4b3c-a3d6-e0321da40636)<br>

To fix that run:
```
$ npm audit fix --force
```
![image](https://github.com/4aiman/slowcam/assets/2913210/53e043ea-4571-4707-9f02-3a8bb00b1077)

Nw just open in a browser:
```
$ chrome index.html
```
Slowcam is written in vanilla Javascript, you don't need to build/transpile any thing.
Opening the `index.html` in your favorite browser is what makes it run.
