# onRobot

Developed at The University of York

A simple gripper library to use a Universal Robot with an onRobot gripper, no onrobot compute box needed.

# Supported onRobot Grippers

- [x] RG2
- [x] VG10
- [ ] Gecko
- [ ] SG
- [ ] TFG
- [ ] SDR
- [ ] 2FG
- [ ] MG
- [ ] FGP

# Installation

```bash
git clone https://github.com/Intelligent-Robotics/onRobot.git
cd onRobot
pip install .
```

# Example Usage

```python
import onRobot.gripper as gripper

rg_id = 0
ip = "192.168.56.101"
rg_gripper = gripper.RG2(ip,rg_id)

rg_width = rg_gripper.get_rg_width()
print("rg_width: ",rg_width)

target_width = 40.00
target_force = 40.00

rg_gripper.rg_grip(target_width, target_force)
```

# Functions implemented for the RG2

- [ ] rg_stop
- [x] rg_grip
- [ ] rg_calibration
- [ ] rg_get_all_variables
- [ ] rg_get_all_double_variables
- [ ] rg_get_all_integer_variable>
- [ ] rg_get_all_boolean_variable>
- [ ] rg_get_speed
- [ ] rg_get_depth
- [ ] rg_get_relative_depth
- [ ] rg_get_angle
- [ ] rg_get_angle_speed
- [x] rg_get_width
- [ ] rg_get_fingertip_offset
- [ ] rg_get_status
- [ ] rg_get_busy
- [ ] rg_get_grip_detected
- [ ] rg_get_s1_pushed
- [ ] rg_get_s1_triggered
- [ ] rg_get_s2_pushed
- [ ] rg_get_s2_triggered
- [ ] rg_get_safety_failed
- [ ] rg_set_fingertip_offset


# Functions implemented for the VG10
- [x] vg10_grip
- [x] vg10_release
- [ ] vg10_idle
- [ ] vg10_get_vacuum
- [ ] vg10_get_all_double_variables