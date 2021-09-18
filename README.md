# 코로가 - 내 위치의 거리두기 단계 😷
위치 액세스를 기반으로 현 위치의 코로나 거리두기 단계 및 모임 가능 인원 수 , 모임 가능 시간을 한 눈에 볼 수 있는 앱입니다.       

![광고모음](https://user-images.githubusercontent.com/71416677/133873314-46ae74ba-adda-4dcb-a865-10fbaf5ef584.jpg)         

## Architecture Pattern
MVC (Model - View - Controller)  

## Access Permission
ACCESS_FINE_LOCATION    
ACCESS_COARSE_LOCATION     
[위치 기반 Access]

## Using
Shared Preferences를 통해 초기 교육용 팝업 visible 여부 판단

## 고찰
1. 활용 할 만한 공공데이터 open api가 마땅치 않아 네트워크 통신이 일체 들어가지 않았습니다.    
2. 네트워크 통신, 로컬 데이터 등을 사용하지 않아 MVVM을 사용하는 것은 오버헤드라고 판단, 결국 MVC 패턴으로 갈아치우고 구현했습니다.    
3. 처음 본 앱을 구상 할 때는 MVVM 패턴을 연습하는 것이 목적이었는데, 실패실패 대실패    
4. 사용한 라이브러리도 오직 Shared Preferences로 Boolean 값 하나만 저장하는 것만 이용했습니다.    
5. 결과적으로 Architecture Pattern을 연습했다기보단 UI/UX 쪽에 집중할 수 있었던 프로젝트 였습니다.    
+ 😷 플레이스토어에 코로나 관련 앱은 등록하지 못한다는 걸 완성하고 깨달았습니다. 😷
