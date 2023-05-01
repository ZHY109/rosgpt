# rosgpt

## Introduction
This project is a simple app of chatGPT in ros, allows you deploy into your robot

## Install 
### Python>=3.8
1. pip install openai

### Python<3.8
1. download a Python>=3.8 and install (suggest python3.8).
2. pip install openai

## How to launch it
1. edit src/rosgpt/scripts/rosgpt.py
2. fill your api_key in "openai.api_key"
3. catkin_make this project
4. roslaunch rosgpt rosgpt.launch

## How to use it
Pub topic /Question with msg type String to get respond:
Example: 
### rostopic pub /Question std_msgs/String -- 'How are you?'
