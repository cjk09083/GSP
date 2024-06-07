

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
<div align="center" >
<img src="https://github.com/cjk09083/GSP/blob/main/모니터링%20APP/1.로그인.png" width="30%"/>&nbsp;
</div></br>

### 장비리스트) GNSS, RTK 장비 목록과 상태 표시
<div align="center" >
<img src="https://github.com/cjk09083/GSP/blob/main/모니터링%20APP/2.장비리스트.png" width="50%"/>&nbsp;
</div></br>

### 상대좌표) 격자 차트 위에 측위 경로 표시
<div align="center" >
<img src="https://github.com/cjk09083/GSP/blob/main/모니터링%20APP/3.상대좌표.png" width="80%"/>&nbsp;
</div></br>

### 지도) 지도상에 GNSS 측위 경로 표시 
<div align="center" >
<img src="https://github.com/cjk09083/GSP/blob/main/모니터링%20APP/4-1.지도화면.png" width="80%"/>&nbsp;
</div></br>

### 데이터목록) 선택한 장비에서 업로드된 측위 데이터 목록 조회 
<div align="center" >
<img src="https://github.com/cjk09083/GSP/blob/main/모니터링%20APP/5.데이터목록.png" width="70%"/>&nbsp;
</div></br>



## 주요 문제점 및 해결방법
- 웹뷰에 지도를 생성한뒤 모바일로 보면 글자와 point들의 크기가 너무 작은 문제 </br>
=> 모바일 기기가 인식되면 Javscript로 CSS를 변경해 차트와 글씨 크기와 위치를 화면크기에 맞게 변경

- 데이터가 500만건을 넘어갈때 데이터 목록 조회 속도 저하</br>
=> 장비별 마지막 ID와 인덱싱을 사용해 조회 속도 개선
