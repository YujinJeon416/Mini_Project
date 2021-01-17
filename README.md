# Mini_Project
 ---------------------------------------

# 1. PREVIEW & 개요
### KH 정보 교육원의 웹 개발자 양성 과정 중 2021년 1월 13일부터 2021년 1월 20일까지 진행되었던 미니 프로젝트의 결과물로, JAVA SWING 으로 구현한 음악재생플레이어입니다.

# 2. 개발동기
- 평소 음악에 관심이 많아서 음악 소프트웨어를 만들고 싶다는 생각이 가장 먼저 들었습니다. 그래서 그런지 음악을 주제로 브레인스토밍을 했을 때 리듬게임에서 작곡 프로그램까지 흥미진진한 것들이 많이 나왔습니다. 그런데 개개인의 역량과 주어진 시간, 사용자 편의성을 생각했을 때. 위의 두 개는 부적합하다고 판단이 되어 뮤직 플레이어를 만들게 되었습니다.
 
 ---------------------------------------
# 3. 제공 기능

   제공 기능              구현 여부   
mp3 확장자 재생               ●   
제목, 가수명 출력             ●   
볼륨 조절                     ●   
재생 시간 표시                ●   
타임 슬라이더                 ●   
배속 재생 -> 곡 이동        X -> ●   
순차, 랜덤, 반복 재생         ●   
가사창                        ●   
플레이 리스트                 ●   



 ---------------------------------------
# 4. 프로젝트 요구사항
- 하나 또는 여러 개의 파일을 재생목록에 추가한다.   
- 재생목록에 있는 파일을 재생, 정지한다.
- mp3 파일의 태그를 추출한다.
- 재생 중인 음악의 제목, 가수명, 전체 재생시간을 표시한다.
- 실시간으로 음악이 재생되는 부분을 숫자와 슬라이더 움직임으로 표시한다.
- 재생할 부분을 조절할 수 있는 슬라이더를 제공한다.
- 재생 중 이전/다음 음악으로 넘어갈 수 있는 기능을 제공한다.
 ---------------------------------------
 # 5. 역할 및 담당 기능
 - 박정현   
  역할: 팀장   
  담당 기능: 음악재생, 멈춤기능, 음악리스트, 음악태그, Swing구현, 코드최적화, 주석작업   
  
- 장호재   
  역할: 팀원   
  담당 기능:   
  
- 전유진   
  역할: 팀원   
  담당 기능: 제목별, 가수별 검색 구현, 회의내용 정리, 백그라운드 이미지 제작, 기획안 작성   
 
 ---------------------------------------
 # 6. 개발 목표 및 설계 주안점
 - 처음 목표는 음악 재생과 정지, 그리고 마이 플레이리스트 기능이었다. 하지만 전부 구현이 가능해지자 욕심이 생겨서 어쩌구저쩌구~........   
 - 사용자 친화적인 인터페이스와 간단한 조작방법을 설계의 주안점으로 두어 최대한 심플한 구성으로 만들기 위해 노력하였다.    
   컨셉은 옛날에 인기가 많았던 Winamp로 잡아 Winamp의 기본 스킨 이미지를 차용하여 백그라운드 이미지를 제작하였고 화면구성도 비슷하게 잡아보았다.      
 ---------------------------------------
 
 
# 7. 핵심 구현 기술   
①재생목록에서 파일을 선택하고 <재생/정지> 버튼을 클릭하면 선택된 파일이 처음부터 재생된다.   
재생되는 동안 파일의 이름, 가수명의 내용이 보여진다. 또한 실시간으로 현재 재생 중인 부분과 전체 재생시간이 숫자와 <시간> 슬라이더로 표시된다.   
②<재생/정지> 버튼을 클릭하면 파일이 멈춘다. 이 상태에서 <재생/정지> 버튼을 다시 클릭하면 파일이 멈춘 지점부터 재생된다.   
③<정지> 버튼을 클릭하면 파일이 멈춘다. 이 상태에서 <재생> 버튼을 클릭하면 파일이 처음부터 재생된다.   
④<다음> 버튼을 클릭하면 현재 재생 중인 파일이 멈추고 재생목록에서의 다음 파일이 처음부터 재생된다.   
⑤재생목록에서의 다음 파일이 없다면 정지된다.   
⑥<이전> 버튼을 클릭하면 현재 재생 중인 파일이 멈추고 재생목록에서의 이전 파일이 처음부터 재생된다.   
⑦재생목록에서의 이전 파일이 없다면 정지된다.   
⑧<시간> 슬라이더를 움직이면 그에 따라 재생 중인 부분이 조절된다.   
⑨순차재생 상태일 경우 재생목록에서의 다음 파일이 처음부터 재생된다.   
⑩랜덤재생 상태일 경우 이제 막 재생을 끝낸 파일을 제외한 재생목록 안 파일 중 임의로 선택된 파일이 처음부터 재생된다.   
⑪반복재생 상태일 경우 이제 막 재생을 끝낸 파일이 처음부터 재생된다.   
⑫리스트에서 추가를 누르면 마이 플레이리스트가 만들어지며 내가 추가한 곡만 재생을 할 수 있다.   
⑬제거를 누르면 마이 플레이리스트에서 제거가 된다.   
⑭   

 ---------------------------------------
# 6. 구현 기간   
### 프로젝트 기획 기간 2021/01/13~2021/01/14   
### 프로젝트 구현 기간 2021/01/14~2021/01/20    
 ---------------------------------------
# 7. 사용 언어 및 도구   
### O/S : Windows 10   
### 개발 언어: Java(JSP)   
### IDE:  Eclipse    
### 라이브러리: jaudiotagger-2.2.6-SNAPSHOT.jar,jl1.0.1.jar    
 ---------------------------------------
# 8. 프로젝트 참여 소감   

 ---------------------------------------
