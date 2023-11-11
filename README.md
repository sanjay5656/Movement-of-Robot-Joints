# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```python
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
pos = [[1,30],[2,40],[3,90]]
robot = getRobot()
robot.driveJoints (0,0,0,0,0,0)
delay(5)
for i in pos:
robot.Controller.moveJoint (i[0],i[1])
delay (5)
```
## Output
### 1. Generic Articulated Robot
![image](https://github.com/sanjay5656/Movement-of-Robot-Joints/assets/115128955/73c8ccf0-7993-4507-b100-872ed2d26d39)

### 2. robot.driveJoints(0,0,0,0,0,0)
![image](https://github.com/sanjay5656/Movement-of-Robot-Joints/assets/115128955/e1d2e1bb-8082-49ad-9389-d3fc75571841)

### 3. Movement of Joint1
![image](https://github.com/sanjay5656/Movement-of-Robot-Joints/assets/115128955/486c62bc-eb23-47be-871f-a0d0d355eda4)

### 3. Movement of Joint2
![image](https://github.com/sanjay5656/Movement-of-Robot-Joints/assets/115128955/989acf67-57f0-4da7-9f98-8410739c2f20)

### 3. Movement of Joint3
![image](https://github.com/sanjay5656/Movement-of-Robot-Joints/assets/115128955/f1162c4a-4873-4cfd-939b-32f8742d7d55)

## Result 
Thus the different robots joints are moved with the help of python list.


