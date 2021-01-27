# mmPose
An Open-Source Toolbox for Human Pose Estimation using mmWave Radars
---
#### PI: [Dr. Siyang Cao](https://uweb.engr.arizona.edu/~caos/)
#### Project Members: [Arindam Sengupta](https://github.com/senguptaa) & [Feng Jin](https://github.com/fengjin-uofarizona)
#### Organization: University of Arizona
#### E-mail: {caos, sengupta, fengjin}@email.arizona.edu
---
# Motivation
While vision based sensors provide a high-resolution representation of the scene, there are a few challenges associated with their operation. They heavily rely on (or influenced by) external sources for illuminating the scene and are therefore rendered ineffective in poor lighting conditions, adverse weather conditions or when the scene/target is occluded. These could result in irrevocable catastrophic events similar to the ones encountered at (i) Tesla's autopilot testing, where the vision sensors failed to detect the white side of a tractor trailer in brightly lit sky (very high reflectivity) , and (ii) Uber self-driving vehicle crash incident in Arizona due to the vision/LiDAR sensors' inability to detect the pedestrian in time to avoid the accident during a night test (low/no reflectivity). There is therefore an imminent need for alternate sensors to achieve the task, while overcoming the aforementioned challenges.

<p align="center">
    <img src="https://media.giphy.com/media/emLsQYHXbStkvKSHty/giphy.gif", width="480">
    <br>
    <sup>Uber Autonomous Car Crash in Arizona, 2018. <a href="https://www.youtube.com/watch?v=RASBcc4yOOo" target="_blank">Source</a></sup>
</p>

Radio Frequency (RF) based sensors, such as radars, use its own signals to illuminate the target (active sensing), therefore making it operationally robust to scene lighting and weather conditions. However, unlike vision based sensors, radars represent the scene using RF intensity based spatial heat-maps, reflection point clouds or range-doppler maps, rather than a true-color image representation. Radars are therefore primarily used for target localization and tracking applications. Furthermore, object classification becomes non-trivial with radar data, and the lack of available labeled radar data-sets for this task makes it even more challenging. 

Traditionally, radar systems have been size and cost intensive primarily targeted to commercial and defense applications. However, continuing advancement in micro-electronics fabrication and manufacturing techniques, including Radio Frequency Integrated Circuits (RFICs), have significantly reduced the size and cost of electronic sensors making them more accessible to public. mmWave automotive radars are an example of this technology. They are low-power, compact and are extremely practical to deploy. Furthermore, mmWave radars provide us with a high resolution point cloud representation of the scene and have therefore emerged as one of the primary sensors in autonomous robots on a smaller scale, to more commercial applications such as autonomous vehicles. Higher operating bandwidths also allow mmWave radars to roughly generate the contour of human body without extracting facial information, thus preserving user privacy.

Therefore, we propose mm-Pose, a novel real-time approach to estimate and track human skeleton using mmWave radars and convolutional neural networks (CNNs). A potential depiction of its application in healthcare through patient monitoring systems is shown below.

<p align="center">
    <img src="https://github.com/radar-lab/mmpose/blob/master/Misc/mmPose.png", width="960">
    <br>
    <sup>mm-Pose can be used in automated patient monitoring systems especially with the shortage in nursing aided supervised care. <a href="https://www.ncbi.nlm.nih.gov/books/NBK493175/" target="_blank">Source</a> </sup>
</p>

To the best of the our knowledge, this is the first method that uses mmWave radar reflection signals to estimate the real-world position of >15 distinct joints of a human body. mm-Pose could also find applications in (i) autonomous vehicles and traffic monitoring systems for pedestrians, and (ii) aiding defense forces in a hostage situation. Radars carrying this technology on unmanned aerial vehicles (UAVs) could scan the building and map the live skeletal postures of the hostage and the adversary, through the walls, which would not have been possible otherwise with vision sensors.

<p align="center">
    <img src="https://github.com/radar-lab/mmpose/blob/master/Misc/mmpose.gif", width="960">
    <br>
    <sup>mmPose output compared to ground-truth for a person walking</sup>
</p>

---
# [Publication](https://ieeexplore.ieee.org/abstract/document/9083948)
Please cite the paper in the following format:

A. Sengupta, F. Jin, R. Zhang and S. Cao, "mm-Pose: Real-Time Human Skeletal Posture Estimation Using mmWave Radars and CNNs," in IEEE Sensors Journal, vol. 20, no. 17, pp. 10032-10044, 1 Sept.1, 2020, doi: 10.1109/JSEN.2020.2991741.

---
# Data-sets and Source Code
Work in progress! Please stay tuned to updates on this repo.



