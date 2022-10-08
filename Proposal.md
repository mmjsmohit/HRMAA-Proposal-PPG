# Proposal for HRMAA - PPG Technology

## What is PPG?

PPG stands for photoplethysmogram. IT can be used to detect blood volume changes in the microvascular bed of tissue.The volume changes are detected by first illuminating the tissues through a light source (such as an LED), and then capturing the reflected light, and then analyzing it. The variations in the light intensity are related to changes in the blood
perfusion of the tissue, and based on these changes heart-related information can be retrieved.
PPGs can be obtained from transmissive absorption (as at the fingertip) or reflection (as on the forehead). <br /><br />

<p align="center">
  <img width="500" height="300" src="https://upload.wikimedia.org/wikipedia/commons/4/4f/PPG.PNG">
</p>
<p align = "center">
Representative PPG taken from an ear pulse oximeter.
</p> <br />

## Current Status of PPG in HRMAA:

Currently, PPG is implemented by using an open source repository called HeartBeat. This project uses a deprecated version of Camera API and is written in Java.
Thus, it was not possible to use this repository as is and hence it was migrated to use Kotlin and an updated version of Camera API called Camera2 API.
As far as accuracy of the data is concerned, the current accuracy measure stands at ±10 BPM. This is the data measured under ideal conditions. Ideal conditions include absolutely stable finger position, light source not too far away from fingertip and heart rate not more than 120 BPM.

