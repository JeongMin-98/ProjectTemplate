# 차선인식 경진대회
본 프로젝트를 진행하기 전까지
- OpenCV 기초와 응용
- 허프변환 기반 차선 인식 주행
- 슬라이딩 윈도우 기반 차선 인식 주행
- 필터 기반 조향각 제어
- PID 기반 조향각 제어
위 내용으로 학습을 진행하며 차선 이탈 없이 자율 주행하기 위해 모든 조원들이 머리를 맞대고 열심히 실습을 진행했습니다. 위의 학습한 내용을 바탕으로 차선인식 경진대회에서 자이카가 차선을 이탈하지 않고 주행할 수 있도록 주어진 템플릿을 활용해서 프로젝트를 진행하시면 됩니다. 주어진 템플릿에 대한 간략한 설명을 읽고 템플릿을 수정하면서 원하는 주행을 할 수 있는 코드를 작성해주세요.

# 템플릿 설명
템플릿의 이름을 LaneKeepingSystem으로 변경한 다음 자이카의 xycar_ws의 src에 업로드하여 catkin_make를 하면 프로젝트의 템플릿으로 활용할 수 있습니다.
## CMakeLists.txt
프로젝트 코드를 Build하는 환경을 설정합니다. 프로젝트를 수행하기 위해서 필요한 패키지, 헤더 파일, 라이브러리, 파일 이름 등을 명시할 수 있으며 필요한 경우 ROS에서 지원하는 msg들을 추가하여 노드 간의 통신 형태를 추가할 수 있습니다.
![code](https://github.com/ihmmaru99/ProjectTemplete/assets/109266664/c17aac73-b4ea-48ff-8552-642f18759745)<br>
기본 Libray
- LaneDetector
- LaneKeepingSystem
- MovingAverageFilter
- PIDController
기본 Package
- OpenCV
- YAML_CPP
- Catkin
- roscpp
- xycar_msgs
- sensor_msgs
- std_msgs
기본으로 탑재된 Library와 Package만으로도 프로젝트를 수행하는데 무리가 없으나 필요한 경우 원하는 패키지 및 라이브러리를 추가하여 사용할 수 있습니다.

