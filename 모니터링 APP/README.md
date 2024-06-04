

# GSP 모니터링 APP 
<div>
<img src="https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=Android&logoColor=white"/> 
<img src="https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=Flutter&logoColor=white"/>
<img src="https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=Dart&logoColor=white"/>
<img src="https://img.shields.io/badge/HTML-E34F26?style=flat-square&logo=HTML5&logoColor=white"/>
<img src="https://img.shields.io/badge/Javascript-F7DF1E?style=flat-square&logo=javascript&logoColor=black"/>
<img src="https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=PHP&logoColor=white"/>
<img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=MySQL&logoColor=white"/>
</div>

## 목적
- GNSS 안테나 및 RTK 수신기 모니터링 
- Flutter + WEB 앱 개발

## 기능 
### 로그인) 모니터링 서버에 등록된 계정으로 접속 
- 사이드 메뉴에서 농장 선택 시 빠른 이동
<div align="center" >
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/0.%20로그인.jpg" width="30%"/>&nbsp;
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/1.%20메인.jpg" width="30%"/>&nbsp;
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/2-1.%20사이드바.jpg" width="30%"/>&nbsp;
</div></br>

### 장비리스트) 날짜별 장비상태 상세정보 출력
<div align="center" >
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/2.%20장비상태.jpg" width="30%"/>&nbsp;
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/2-1%20장비상태%20-%20날짜선택.jpg" width="30%"/>&nbsp;
</div></br>


### 상대좌표) 기간별, 항목별 수치 그래프로 출력
<div align="center" >
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/2-2%20그래프%20(일반).jpg" width="30%"/>&nbsp;
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/2-2%20그래프%20(풍향풍속).jpg" width="30%"/>&nbsp;
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/2-2%20그래프%20종류.jpg" width="30%"/>&nbsp;
</div></br>

### 지도) 일반/위성 지도로 일별 농장 정보 출력 
<div align="center" >
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/2-3%20대기확산(일반).jpg" width="30%"/>&nbsp;
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/2-3%20대기확산(위성).jpg" width="30%"/>&nbsp;
</div></br>

### 데이터목록) 선택한 장비에서 업로드된 측위 데이터 목록 조회 
<div align="center" >
<img src="https://github.com/cjk09083/GSP/blob/main/모니터링%20APP/5.데이터목록.png" width="70%"/>&nbsp;
</div></br>



## 주요 문제점 및 해결방법
- 웹사이트로 풍향/풍속 차트를 생성후 모바일 화면에 웹뷰어 형태로 출력시 차트와 글씨가 너무 작아지는 문제 </br>
=> 모바일 기기가 인식되면 Javscript로 CSS를 변경해 차트와 글씨 크기와 위치를 화면크기에 맞게 변경

- 데이터가 500만건을 넘어갈때 데이터 목록 조회 속도 저하</br>
=> Map 위에 레이어를 씌워 1차적으로 레이어에서 터치와 스크롤을 처리하고 이를 하위의 Map에 전달해 전체 페이지와 Map을 연동
