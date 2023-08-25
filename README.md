# Back-end-Exercise
>Back-end Server 한이음 실제 사용 서버이다.

## 1_login 연결
Front와 Back login 및 signup을 연결한 코드이다.
1. 기본 시작-/member/login </br>
  1-1. 계정생성 필요 시 아래 버튼 클릭 ->signup으로 넘어감 </br>
  1-2. 접속 시 저장된 계정만 접근 가능 ->id, password 입력 후 로그인 클릭 </br>
2. 회원 가입-/member/signup </br>
  2-1. name, userId, user_password로 가입 가능 ->login으로 넘어감 </br>
  2-2. 만약 계정이 있으면 ->바로 login으로 이동 </br>
3. main-/main </br>
로그인 성공 시 main페이지 진입 </br>

4. 관리자 접근-/admin/list </br>
가입한 회원 목록 확인 가능 </br>
삭제 선택 시 팝업창 띄운 후 삭제 </br>

## 2_Data 연결
실시간 수집 데이터 모체로봇에서 서버로 송신하여 저장하는 코드이다. </br>
1. 소형 로봇 온습도 센서에서 10초마다 수집, 모체 로봇으로 전송 </br>
2. 모체 로봇에서 2분마다 서버(MySQL)에 저장 </br>
3. 온도 그래프 및 습도 그래프가 데이터가 바뀔때마다 변함 - /data/mrobot </br>

## 3_Video 연결
스트리밍 영상 관련 video DB에 저장 및 출력 코드이다. </br>
1. 컴퓨터에 기존 가진 비디오 영상 파일을 DB에 저장- /video/insert </br>
2. DB에 저장된 비디오 목록을 불러와 데이터 테이블에서 확인 - /video/list </br>
3. 엔드포인트에서 json 형식의 목록 확인 - /video/getFilesList </br>

## 4_Navigation 연결
네비게이션 바 클릭 시 해당 페이지로 이동하는 코드이다. </br>
1. logo.png 클릭 시 main으로 이동 </br>
2. 홈 클릭 시 main으로 이동 </br>
3. 실시간 정보 클릭 시 streaming or location으로 이동 </br>
4. 재난지역 클릭 시 disaster로 이동 </br>
5. 컨트롤러 클릭 시 controller로 이동 </br>
6. 로봇 데이터 클릭 시 robot or srobot으로 이동 </br>
7. 영상 데이터 클릭 시 video로 이동 </br>
