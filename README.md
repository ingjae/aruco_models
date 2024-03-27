gazebo_models
==============


Dependancy
---
```
sudo apt install graphicsmagick-imagemagick-compat
```


How to use
----------
### 
```
cd {PATH_TO_CLONE}
git clone https://github.com/ingjae/aruco_models
```
### 마커 모델 생성 
```
cd {PATH_TO_CLONE}
cd aruco_models/ar_tags/scripts
./generate_markers_model.py -i {image_path} -s 1000 -w 500
```
image_path 예시 : ```~/catkin_ws/src/aruco_models/ar_tags/images```



### 가제보에 추가 하는 방법
- 가제보 world 실행 (turtlebot3 house 등)
- ```insert``` tap 클릭 후 Marker0, Marker1 추가 (0,1 만 쓸것)  
![image](https://github.com/ingjae/aruco_models/assets/52307552/898745c5-2b4e-4fce-9135-934b97c0ba74)  

- 마커 한변의 길이는 50cm로 생성됨  
![image](https://github.com/ingjae/aruco_models/assets/52307552/51ce3fdf-bae9-4b9e-8890-4b49782d66cb)  


### 마커 모델 제거 방법 
```
cd ~/.gazebo/models
sudo rm -rf marker*
```
