gazebo_models
==============


Dependancy
---
```
sudo apt install graphicsmagick-imagemagick-compat
```


How to use
----------
### 마커 생성 
```
cd PATH_TO_CLONE/aruco_models/ar_tags/scripts
./generate_markers_model.py -i {image_path} -s 1000 -w 500
```
image_path 예시 : ```~/catkin_ws/src/aruco_models/ar_tags/images```

### 마커 제거 후 다시 추가 
```
cd ~/.gazebo/models
sudo rm -rf marker*
```

### 가제보에 추가 하는 방법
- 가제보 world 실행 (turtlebot3 house 등)
- insert tap 클릭 후 Marker0, Marker1 추가 (0,1 만 쓸것)

