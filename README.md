# Project #1 (KIDA)

### 아키
  1. 도커 사용하여 opencv 구축
  2. 아래 사이트1 참고하여 age prediction 웨잇 작성 및 저장
  3. 라즈베리파이에 웨잇 직접 넣기
  4. 라즈베리파이 실행 및 테스트
  5. 비접촉 온도 센서 if 문 활용 코드 첨가
  6. 부분 수정 및 전체 실행
  7. 앱이나 웹사이트 폰 연결(알림)


### 작동 방식
  1. 비접촉 온도센서가 섭씨 50도 이상 감지할 때 true
  2. 카메라 실행
  3. 페이스 디텍션
  4. 어른 아이 구분
  5. 아이 인식 시 부저 경고
  6. 바로 부모에게 스마트폰 알림 경고


#### 사용할 코드/사이트
 1. https://www.learnopencv.com/age-gender-classification-using-opencv-deep-learning-c-python/
 2. https://de.slideshare.net/pyrasis/docker-fordummies-44424016 --> 도커 사용
 3. https://www.dropbox.com/s/xfb20y596869vbb/age_net.caffemodel?dl=0 --> age prediction
 4. run code "python AgeGender.py --input <input_file>(Leave blank for webcam)" --> age prediction (사이트3)
 5. github learnopencv 참고
 6. https://webnautes.tistory.com/916 --> opencv
 7. https://blog.naver.com/aul-_-/221784058038

! ls /weight/age_net.caffemodel


# Todo
## from 2020.03.31
* 아키 다이어그램
* 소스코드 정리(특히 코랩 부분)
* 라즈베리파이 부분 완성
* 추가 Traing 코드 Colab에서 구현

# Done
* Aws 중계 서버 구축(AMI:NGINX)
* Raspberry에 Implementation 환경 구현(OpenCv + Camera모듈  + 코드적용 )

### Next Todo
* Raspberry →(오작동 데이터:이미지,레이블 by scp)→ AWS ← CoLab에서 수동으로 폴링, Train 끝나면 Weight 정보 수정 Upload with 버전과 함께
* Raspberry 주기적으로 Weight 업데이트
