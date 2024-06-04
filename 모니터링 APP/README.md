

# ATD iOS/Android APP 
<div>
<img src="https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=Android&logoColor=white"/>
<img src="https://img.shields.io/badge/iOS-000000?style=flat-square&logo=Apple&logoColor=white"/>  
<img src="https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=Flutter&logoColor=white"/>
<img src="https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=Dart&logoColor=white"/>
<img src="https://img.shields.io/badge/HTML-E34F26?style=flat-square&logo=HTML5&logoColor=white"/>
<img src="https://img.shields.io/badge/Javascript-F7DF1E?style=flat-square&logo=javascript&logoColor=black"/>
<img src="https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=PHP&logoColor=white"/>
<img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=MySQL&logoColor=white"/>
</div>

## 목적
- 축산농장 모니터링 및 작업내역 업로드 
- Flutter로 iOS, Android 하이브리드앱 개발 및 배포

## 기능 
### 메인) 로그인 후 농장별 서버와 연동하여 최신상태 출력 
- 사이드 메뉴에서 농장 선택 시 빠른 이동
<div align="center" >
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/0.%20로그인.jpg" width="30%"/>&nbsp;
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/1.%20메인.jpg" width="30%"/>&nbsp;
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/2-1.%20사이드바.jpg" width="30%"/>&nbsp;
</div></br>

### 장비상태) 날짜별 장비상태 상세정보 출력
<div align="center" >
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/2.%20장비상태.jpg" width="30%"/>&nbsp;
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/2-1%20장비상태%20-%20날짜선택.jpg" width="30%"/>&nbsp;
</div></br>


### 그래프) 기간별, 항목별 수치 그래프로 출력
<div align="center" >
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/2-2%20그래프%20(일반).jpg" width="30%"/>&nbsp;
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/2-2%20그래프%20(풍향풍속).jpg" width="30%"/>&nbsp;
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/2-2%20그래프%20종류.jpg" width="30%"/>&nbsp;
</div></br>

### 대기확산) 일반/위성 지도로 일별 농장 정보 출력 
<div align="center" >
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/2-3%20대기확산(일반).jpg" width="30%"/>&nbsp;
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/2-3%20대기확산(위성).jpg" width="30%"/>&nbsp;
</div></br>

### 작업내역) 농장에서 진행한 작업 정보를 서버와 연동 
<div align="center" >
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/2-4%20작업내역.jpg" width="30%"/>&nbsp;
<img src="https://github.com/cjk09083/ATD/blob/main/IOS%26Android%20APP/2-4%20작업등록.jpg" width="30%"/>&nbsp;
</div></br>



## 주요 문제점 및 해결방법
- 웹사이트로 풍향/풍속 차트를 생성후 모바일 화면에 웹뷰어 형태로 출력시 차트와 글씨가 너무 작아지는 문제 </br>
=> 모바일 기기가 인식되면 Javscript로 CSS를 변경해 차트와 글씨 크기와 위치를 화면크기에 맞게 변경

- Google, Naver Map 사용시 전체 페이지 터치와 스크롤이 연동되지 않는 문제</br>
=> Map 위에 레이어를 씌워 1차적으로 레이어에서 터치와 스크롤을 처리하고 이를 하위의 Map에 전달해 전체 페이지와 Map을 연동
