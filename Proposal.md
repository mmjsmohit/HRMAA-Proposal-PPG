# Proposal for HRMAA - PPG Technology

## What is PPG?

PPG stands for photoplethysmogram. IT can be used to detect blood volume changes in the microvascular bed of tissue.The volume changes are detected by first illuminating the tissues through a light source (such as an LED), and then capturing the reflected light, and then analyzing it. The variations in the light intensity are related to changes in the blood
perfusion of the tissue, and based on these changes heart-related information can be retrieved.
PPGs can be obtained from transmissive absorption (as at the fingertip) or reflection (as on the forehead).

<p align="center">
  <img width="500" height="300" src="https://upload.wikimedia.org/wikipedia/commons/4/4f/PPG.PNG">
</p>

<p align = "center">
Representative PPG taken from an ear pulse oximeter.
</p>


## Current Status of PPG in HRMAA:

Currently, PPG is implemented by using an open source repository called HeartBeat. This project uses a deprecated version of Camera API and is written in Java.
Thus, it was not possible to use this repository as is and hence it was migrated to use Kotlin and an updated version of Camera API called Camera2 API.
As far as accuracy of the data is concerned, the current accuracy measure stands at ±10 BPM. This is the data measured under ideal conditions. Ideal conditions include absolutely stable finger position, light source not too far away from fingertip and heart rate not more than 120 BPM.

## Goals by the end of this project:
- [ ] Studying the scope of Camera2 API.
    - [ ] Understanding the [Official Documentation](https://developer.android.com/reference/android/hardware/camera2/package-summary) and [training modules](https://developer.android.com/training/camera2).
    - [ ] Creating some dummy applications to test the utilities such as Image Processing and Image Manipulation.
- [ ] Bring down the error from ±10 BPM to less than or equal to ±5 BPM.
    - [ ] Investigating the cause of mentioned error.
    - [ ] Refering to existing and similar apps for solution.   
    - [ ] Finding ways to analyze the camera input more accurately. 
- [ ] Overcoming the difficulties caused by non-ideal conditions.
    - [ ] Implement a user education module which teaches the user on how to use the PPG Feature.
    - [ ] Finding a method to detect abnormal conditions and notifying the user about them.
- [ ] Coordinating with other verticals to integrate PPG into a production app.
    - [ ] Understanding the requirements and limitations of other verticals for data storage, etc.
- [ ] Working on improving the UI/UX and making the PPG feature more accessible.

<p align="center">
  <img src="https://github.com/mmjsmohit/HRMAA-Proposal-PPG/blob/main/HRMAA.gif" width="300" />
</p>
