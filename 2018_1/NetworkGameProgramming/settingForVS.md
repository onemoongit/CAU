# Visual Studio Setting for NGP

## ws2_32.lib 추가하기

- 프로젝트 속성 -> 링커 -> 입력 -> 추가종속성 에서 편집을 누른 뒤 ws2_32.lib를 추가한다.

## SDL 검사 제거

- C/C++ 파일이 먼저 있어야 한다.
- 프로젝트 속성 -> C/C++ -> SDL검사 -> 아니오 체크

## console 

- 콘솔이 바로 사라지는 경우 
	- 보통 빈 프로젝트로 생성할 시에 결과를 보기도 전에 사라진다
- 프로젝트 속성 -> 링커 -> 시스템 -> 하위시스템 을 콘솔로 변경한다
- main 코드 마지막쯤에 system("pause") 를 삽입한다. 
- ctrl + F5 ( 디버그하지 않고 시작 )을 사용한다.
- 콘솔창이 바로 사라지지 않는다