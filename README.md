# ICARUS- an microsoft imagine cup MVP submission

## Using Matlab Simulations




## PD Controller

- Run code: change trajectories in file `control/runsim.m` and run.
- See `control/controller.m` for implementation of the PD controller.
- Visualization below. Desired (blue) vs Actual (red)

#### Trajectory 1: Step

<img src="gifs/p1p1_step.gif" alt="step" width="270"> <img src="imgs/p1p1_step_p.jpg" alt="step" width="270"> <img src="imgs/p1p1_step_v.jpg" alt="step" width="270">


#### Trajectory 2: Circle

<img src="gifs/p1p1_circle.gif" alt="step" width="270"> <img src="imgs/p1p1_circle_p.jpg" alt="step" width="270"> <img src="imgs/p1p1_circle_v.jpg" alt="step" width="270">

#### Trajectory 2: Diamond

<img src="gifs/p1p1_diamond.gif" alt="step" width="270"> <img src="imgs/p1p1_diamond_p.jpg" alt="step" width="270"> <img src="imgs/p1p1_diamond_v.jpg" alt="step" width="270">

## Path Planning and Trajectory Optimization

- Run code: `traj_planning/runsim.m` and run path 1 or path 3.
- See `traj_planning/path_planning/dijkstra.m` for implementation of path finding algorithms (dijstra, A*).
- See `traj_planning/traj_opt7.m` for implementations of minimium snap trajectory.
- See `traj_planning/traj_opt5.m` for implementations of minimium acceleration trajectory.
- Visualization below.





## App using Yolov5 Real-time Inference using Streamlit

<img src="output.gif" alt="demo of the dashboard" width="800"/>

### [Live Demo](https://moaaztaha-yolo-interface-using-streamlit-app-ioset2.streamlit.app/)


## Features
- **Caches** the model for faster inference on both CPU and GPU.
- Supports uploading model files (<200MB) and downloading models from URL (any size)
- Supports both images and videos.
- Supports both CPU and GPU inference.
- Supports:
  - Custom Classes
  - Changing Confidence
  - Changing input/frame size for videos


## How to run
After cloning the repo:
1. Install requirements
   - `pip install -r requirements.txt`
2. Add sample images to `data/sample_images`
3. Add sample video to `data/sample_videos` and call it `sample.mp4` or change name in the code.
4. Add the model file to `models/` and change `cfg_model_path` to its path.
```bash

cd Yolo-Interface-using-Streamlit
streamlit run app.py
```


