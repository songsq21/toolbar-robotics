# Human to Humanoid

This part serves as the motion capture and retargeting codebase where some algorithms is introduced from other repos.

To start with, you may need to add some data and pre-generated models in the sub-folder `./human_to_humanoid/` to better process the data:

* `./human_model/` contains the pre-trained human motion param models such as SMPL, SMPL-X, etc.
  * You may need to change the name of the `.pkl` files to be supported by python libraries such as `smplx`. Due to the license and file size, the `.pkl` formed motion model are not available here inside the codebase.
  * SMPL model see [SMPL website](https://smpl.is.tue.mpg.de/).
  * SMPL-X model see [SMPLX website](https://smpl-x.is.tue.mpg.de/).
* `./humanoid_model/` contains the humanoid models needed for simulation and kinematics generation.
  * Current Unitree robots see [Unitree RL codebase](https://github.com/unitreerobotics/unitree_rl_gym).
  
## Retarget with On-body Keypoints

