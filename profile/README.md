# Software1 Team Organization
## Projects Repository Naming Conventions

> **`Base model`_`Project Features`**

- `sr3_lse` - LSE 청주 AMR 프로젝트
- `sr5_stator` - 북미 모비스 Stator AMR 프로젝트
- 

## Projects Repository Constructs

### template_repository

- 프로젝트 혹은 로봇 개발을 위해 최소한의 모듈들로 구성된 template, 공통으로 발생하는 문제에 대해 지속적인 관리하며 개선하여 안정화를 진행할 예정. 
- Core 모듈들을 서브모듈로 포함하고 있으며, 로봇에 필요한 패키지들을 추가적으로 포함.

### core repository

서브모듈로 사용되는 레퍼지토리:

- `scorpion_ros`: 로봇 요소의 구동 및 실행, TASK 수행과 관련된 핵심 모듈
- `core_docking`: 도킹과 관련된 핵심 모듈
- `core_localization`: 위치 추정과 관련된 핵심 모듈
- `core_navigation`: 주행과 관련된 핵심 모듈
- `ros_parameters_group`: Syscon 시스템 구성에 필요한 파라미터 집합체 (`RPG`)

**Third_party_group's individual packages**
- `lidar`: 라이다 관련 오픈소스 패키지
- `multimaster_fkie`: 로봇 연결 관련 패키지
- `realsense_ros`: realsense 3D 카메라 관련 패키지
- `rospy_message_converter`: 파이썬 딕셔너리 로스 메시지 변환 관련 오픈소스 패키지
- `service_timeout`: rosservice 비동기 서비스 실행 모듈 
- `syscon_msgs`: 사용되는 메시지 관련 패키지
- `bag_packing`: 디버깅을 위해 사용되는 데이터 저장 관리 패키지
