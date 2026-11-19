# **Machine Learning Engineer** 📈  

- **MEng in Electrical Engineer & Computer Science**  
-  Passionate about machine learning, with expertise in transforming research papers into efficient code implementations, training neural networks, and building real-world AI applications, and deploying them on legged robots (Unitree Go2 & G1).  

## **Experience** 💼
- **Computer Vision Engineer** @ I-SENSEGroup/ICCS, 2025 – Present
•	Implemented a semantic 3D Scene Understanding pipeline, processing LiDAR and depth data from robotic scans.
•	Built a text-to-object retrieval system, enabling natural language queries for 3D environments.
•	Integrated 2D foundation models (DINO, CLIP, SAM) with 3D pipelines for scene interpretation.
•	Applied state-of-the-art methods for large-scale unstructured 3D data processing and vector search over embeddings.

- **Machine Learning Engineer / AI Consultant** @ EY-Greece 🌍
 • Gained in-depth familiarity with NLP concepts and best practices.
 • Implemented GenAI architectures like Multi-Agent Systems, RAG
   and more.
 • APIs and Integration: Designing and implementing RESTful APIs to
   deploy models in production environments.
 • Exploratory Data Analysis (EDA): Strong ability to visualize and
   interpret data to uncover insights.
 • Client-Facing Communication: Experience presenting technical
   findings and recommendations to clients and stakeholders.
  
 - **Diploma Thesis** 📝 – [Deep Learning Video Stabilization](/assets/thesis.pdf):
   
   ![Deep Learning Video Stabilization Result](/assets/img/stab_result.gif)  
   • Gained in-depth knowledge of Computer Vision concepts by implementing and modifying numerous research papers.  
   • Became proficient in Deep Learning training principles and best practices.  
   • Used state-of-the-art techniques such as Deep Perceptual Losses, Transfer Learning, feature embeddings, and fine-tuning.  
   • Leveraged advanced network architectures like channel attention, gated convolutions, and more.  
   • Implemented advanced training schemes such as cGAN, WGAN, Siamese Networks, and more.  
   • Mastered best practices for data preprocessing.  
   • Proposed two novel approaches for generating realistically unstable videos for supervised training:  
     • Approach 1: Trained a model to generate realistic motion noise.  
     • Approach 2: Utilized Principal Component Analysis for noise generation.
   ![DMBVS_UNET Architecture](/assets/img/DMBVS_UNET.png)  

## **Robotics** 🤖
Hands-on work deploying **Unitree Go2 (quadruped)** and **Unitree G1 (humanoid)** robots on real hardware, in **NVIDIA Isaac Sim / Isaac Lab**, and in **Gazebo**, with ROS 2 as the common backbone.

### 🦾 Real robots: SLAM, navigation & skills framework
[**Unitree-Go2-and-G1-SLAM-navigation-and-skills-framework**](https://github.com/btxviny/Unitree-Go2-and-G1-SLAM-navigation-and-skills-framework)

![Real-robot 3D map and costmap](/assets/img/robotics/real_robot_map.png)

- Autonomous mapping and navigation on a real **Go2 EDU** (Hesai XT16 LiDAR, RealSense) and **G1** (Livox Mid360), both running at the same time.
- LiDAR odometry (**KISS-ICP**) + **slam_toolbox** run on the robot's dock inside Docker; **Nav2**, RViz2, frontier exploration and AMCL map-to-map localization run on a workstation over CycloneDDS.
- Localization in a saved global map, offline map building from bags, and a velocity bridge from Nav2 to the Unitree SDK (`SportClient` / `LocoClient`).
- G1 skills: arm kinematics (Pinocchio IK) driven by **QR-code detection** from the head camera, Inspire dexterous hands, text-to-speech and speech-to-text.
- A **FastAPI** service exposing one HTTP contract for both robots plus a **Streamlit** control UI (telemetry, skills, localization, speech) for orchestration.

### 🧪 Isaac Sim: RL locomotion + SLAM-ready office
[**Isaac-Sim-SLAM-with-Go2-and-G1**](https://github.com/btxviny/Isaac-Sim-SLAM-with-Go2-and-G1)

- Trained walking policies for the Go2 and a custom 23-joint G1 with **RSL-RL (PPO)** in Isaac Lab.
- Office scene with simulated RTX lidar and RealSense cameras published to ROS 2 through OmniGraph.
- Policies deployed as separate **ROS 2 nodes** (TorchScript/ONNX), closing the loop over `/obs` and `/joint_commands` at 200 Hz physics.

### 🏢 Gazebo: Go2 office navigation
[**Unitree-Go2-Simulation-in-Gazebo**](https://github.com/btxviny/Unitree-Go2-Simulation-in-Gazebo)

![Go2 driving around the simulated office](/assets/img/robotics/go2_nav_office.gif)

- Go2 with head-mounted RGBD camera and back-mounted 3D lidar in a procedurally generated office (Blender → SDF → Gazebo Harmonic, ROS 2 Jazzy).
- **KISS-ICP** / **FAST-LIO2** odometry, SLAM, **Nav2** point-to-point navigation and autonomous **frontier exploration**.

<p align="center">
  <img src="/assets/img/robotics/kiss_icp_pointcloud_overview.png" alt="Accumulated KISS-ICP point cloud of the office" width="49%">
  <img src="/assets/img/robotics/kiss_icp_pointcloud_robot_closeup.png" alt="Robot navigating inside the accumulated cloud" width="49%">
</p>

**Stack:** ROS 2 (Humble/Jazzy) | Nav2 | slam_toolbox | KISS-ICP | FAST-LIO2 | Gazebo | Isaac Sim / Isaac Lab | RSL-RL | Docker | Unitree SDK2 | FastAPI | Streamlit

## **Education** 🎓  
- **MEng in Electrical Engineering and Computer Science**  
  *University of Patras*  
  *Specialization*: Computer Software & Hardware  
  *Diploma Thesis*: **Deep Learning Video Stabilization**


## **Technical Skills** 🔧
PyTorch | TensorFlow |
Computer Vision | OpenCV | 
Natural Language Processing | RAG | MultiAgent - Applications | Autogen | LangChain | LangGraph |
ROS 2 | Nav2 | SLAM | Isaac Sim | Gazebo | Reinforcement Learning (RSL-RL) |
Distributed Training | Docker | GCP | Azure |
Signal Processing | Matlab | OpenMP | x86 Assembly | Parallel Computing | SQL  


## **Soft Skills** ✨  
*Attention to Detail* | *Leadership* | *Resourcefulness* | *Communication*

## **Projects** 🔍  
![Neural Style Transfer](/assets/img/neural_style.gif)  
![Real-Time Face Verification](/assets/img/faceid.gif)


- 🎥 Implemented various Computer Vision projects such as:  
  - Real-time face verification using pretrained model embeddings.  
  - Semantic segmentation from drone footage.  
  - Neural style transfer and Stable Diffusion models.  
  - Sign language detection using human pose models.  
- 📊 Created numerous Kaggle notebooks on:  
  - Natural Language Processing: User review sentiment analysis.  
  - Time-series forecasting and regression models.


## **Hobbies & Interests** 🎾🎶🔌  
*Tennis* | *Music Playing* | *Electronics* | *Agriculture* | *Cooking*
