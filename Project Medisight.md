# :pushpin: Medisight
>시각장애인을 위한 종합 의료 도우미 서비스  
>https://github.com/GDSC-SWU/2023-Medisight-SolutionChallenge  

</br>

## 1. 대회 정보
Google 기술을 사용하여 UN의 17가지 지속 가능한 개발 목표를 하나 이상을 해결하는 구글 주최 해커톤  
[[대회 정보 링크]](https://developers.google.com/community/gdsc-solution-challenge?hl=ko)

</br>

## 2. 제작 기간 & 참여 인원
- 2023년 1월 23일 ~ 2023년 4월 1일
- 팀 프로젝트, 인원 : 4명

</br>

## 3. 사용 기술
#### `Client`
  - Flutter
  - Firebase
  - Mlkit
  - Google-maps-api  
  - Gradle
#### `Back-end`
  - Nodejs
  - RestAPI
  - Gcp
  - Prisma
  - FastAPI  
#### `ML`
  - Cloud-vision-api
  - Yolov8

</br>

## 4. 핵심 기능
이 서비스의 핵심 기능은 카메라 스캔을 통한 의약품 인식 기능과 유효기간 인식 기능입니다.  
사용자가 바코드를 통해서 의약품을 스캔하면, 의약품 정보가 보여집니다.  
만약 스캔한 사진의 형체를 알아볼 수 없는 등의 기타 오류가 있다면 ML 모델을 통해 재촬영이 필요하다고 안내합니다.  
위 과정은 사진이 서버로 넘어가고 서버에 배포된 ML 모델을 통한 결과를 다시 서버로부터 받아오는 과정을 통해 구현됩니다.  
<p><img width="200" src="https://github.com/jeong-1/jeong-1/assets/68230434/87d941fb-3fe3-4349-9348-301b0d56912a"/></p>
<p><img width="200" src="https://github.com/jeong-1/jeong-1/assets/68230434/2e2e7c04-efd3-4178-ac38-efb1d64cacc8"/></p>

</br>

## 5. 담당 영역
  `Android App Client`

</br>

## 6. 기여
- 안드로이드 환경 구축
- 마이페이지 개발
    - 위젯 생성 및 화면 전환 기능 구현
- 사용자 질환 설정 페이지 개발
    - firebase에서 데이터를 읽고 쓰는 기능 구현
- 카메라 페이지 개발
    - async / await를 활용하여 일정주기마다 스냅샷 촬영 기능 구현
    - ML kit을 사용하여 바코드를 스캔하는 기능 구현
    - rest api를 호출하여 GCP 서버와 통신 구현
