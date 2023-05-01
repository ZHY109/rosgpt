# rosgpt

## Introduction
This project is a simple app of chatGPT in ros, allows you deploy into your robot.

## Install 
### Python>=3.8
1. ```pip install openai```

### Python<3.8
1. download and install Python3.8.
2. ```sudo gedit src/rosgpt/scripts/rosgpt.py``` 
3. The first line should be the location of Python3.8.
4. ```pip install openai```

## How to launch it
1. ```sudo gedit src/rosgpt/scripts/rosgpt.py```
2. fill your api_key in "openai.api_key".
3. ```catkin_make ``` this project.
4.  ```roslaunch rosgpt rosgpt.launch ```

## How to use it
1. Pub topic /Question with msg type String to get respond.
2. Then look at the terminal or  ```rostopic echo /Responce```

### Try this 
 ```rostopic pub /Question std_msgs/String -- 'How are you?' ```
