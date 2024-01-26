## :tada: 쿠팡이츠 클론 코딩 프로젝트 Server [라이징 캠프 13기 테스트]
### ※ 해당 프로젝트의 템플릿에 대한 저작권은 (주)소프트스퀘어드에 있습니다
- - -

## :bulb: 기술 스택
<img src="https://img.shields.io/badge/-SpringBoot-green"/> <img src="https://img.shields.io/badge/-nginx-yellowgreen"/>
<img src="https://img.shields.io/badge/-MySQL-red"/>
<img src="https://img.shields.io/badge/-AWS-orange"/>
<img src="https://img.shields.io/badge/-JWT-blue"/>
<img src="https://img.shields.io/badge/-OAuth-yellow"/>


## :books: [API DOCUMENT](https://docs.google.com/spreadsheets/d/19_krKrCAip0LuEZJsWMf815BNcbxDeia/edit?usp=sharing&ouid=114720192267022828790&rtpof=true&sd=true)


## ERD ![사진](https://user-images.githubusercontent.com/106572156/222183190-bb51c7bf-23ed-4fcd-9010-fc4530222c9e.png)


## :iphone: 시연화면 (Android)
<img src="https://user-images.githubusercontent.com/106572156/222185270-1176a163-d796-4a4e-95c2-27164093b530.PNG"  width="250" height="400"/> <img src="https://user-images.githubusercontent.com/106572156/222187116-f947800f-4c87-41c8-b840-5c33167ee664.png"  width="250" height="400"/> <img src="https://user-images.githubusercontent.com/106572156/222185250-2dfb6675-c168-4dcd-aebf-e30deb61a01a.PNG"  width="250" height="400"/> <img src="https://user-images.githubusercontent.com/106572156/222185265-be403d09-4e5c-4857-9ac0-45d92831e4e0.PNG"  width="250" height="400"/> <img src="https://user-images.githubusercontent.com/106572156/222185277-2a182cbd-d285-4de2-8df3-3d8fad2d7428.PNG"  width="250" height="400"/> <img src="https://user-images.githubusercontent.com/106572156/222187943-9309646a-a331-424e-aaac-df0fff99fb30.png"  width="250" height="400"/>
## 💡 개발일지

### 2022-01-28 (1일차)

1. 기능 구현에 필요한 API 목록 리스트업 및 명세서 양식 작성

2. 화면 구성에 필요한 파라미터 및 리턴값 논의

3. 각자의 깃허브 브랜치 생성

### 2022-01-29 (2일차)

1. 첫주차에 진행할 API에 필요한 파라미터 및 리턴값 형식 논의
- 식당  상세 조회 , 메뉴 상세 조회  API 설계

2. 주요 기능 위주의 ERD 설계 , 초안 구성
  - 유저 , 회원 , 주문 , 리뷰 , 식당 위주로 ERD 구성

3. (개인)식당  상세 조회
  

### 2022-01-30 (3일차)


1. ERD 테이블 연관 관계 설정 , 컬럼 타입 수정 및 보충

2. API url 리스트업 

3. (서버) 메뉴 옵션 처리 구현 방법 관한 회의 진행

4. (개인) 로그인, 회원가입 API 구현

### 2022-01-31 (4일차)
    
1. 프론트와 협의 후 API 명세서 양식 구성과 내용 보충

2. 파라미터 , 리턴값 형식 논의 

3. (서버) 1차 멘토링 전 ERD , REST API 보완 및 질문 리스트 정리
   1. url 에 userId 적합성 포함 여부
   2. 옵션 테이블 구성 방식
   3. 서버 디렉토리 구조 

4. (개인) 식당 상세 조회 , 로그인 , 회원 가입 API 에 관한 더미데이터 추가 

5. (개인)개발 도메인 분리 후 API 배포

### 2022-02-01 (5일차)

#### 1차 피드백 진행
피드백 내용  
>  1. int 데이터 타입은 unsigned int로 변경  
>  2. enum은 관리하기 어려우므로 , 관리하기 힘듦 차라리 varchar 사용 권장      
>  3. 공지사항 내용은 text로 변경  
>  4. 대표자명에 대한 데이터 길이가 너무 짦음  
>  5. 스토어 이미지 테이블 분리 권장  
>  6. 시트에 작업하고 있는 api 구분 권장  
>  7. url에서 유저 id가 꼭 있을 필요는 없다.   
>  8. 서버 디렉토리를 나눌 때는 큰 서비스 단위로 하는 게 바람직  

1. 피드백 내용에 따라 ERD 테이블과 REST API 수정 

2. 메뉴 옵션 테이블 구성 및 구현 방식 논의

3. 메뉴 상세 보기 API 구현

4. 메뉴 상세 보기 , 식당 정보 조회 API 명세서 작성

### 2022-02-02 (6일차)

1.(서버) 코드 merge 일정 조율 및 개발 일정 논의
- 해피 : 홈 화면 구성  API , 리뷰 상세 보기 API 구현
- 개인 : 메뉴 상세보기 API , 주문 생성/조회 API 구현

2. 주문 생성 API 구현

### 2022-02-03 (7일차)

1. (개인)키워드 검색 API 구현
- 각 식당과 식당에 해당하는 메뉴에 키워드가 포함되어 있으면 해당 식당 노출
- 만약 사용자가 로그인이 되있으면 사용자 주소 기반 결과 출력
  로그인이 되어있지 않으면 임의의 gps 좌표값으로 결과 출력

### 2022-02-04 (8일차)

1. (서버) 브랜치 통합 진행 및 메인 브랜치와 merge
   - 처음에 서로 다른 파일에서 시작해서 merge가 되지 않아 진행 X 
2. (서버)rest API 추가 리스트업 erd 테이블 수정

3. API 명세서 작성

### 2022-02-05 (9일차)

1. 그동안 작업한 API 코드 보완 및 기능 수정
- JWT 토큰 인증 적용
- 코드 수정

2. API 명세서 작성 

3. API 서버 반영 , 무중단 서비스 (NO HUP) 적용

### 2022-02-06 (10일차)

1. 클라이언트와 2차 위클리 스크럼 진행
  - api 연동 계획 , 개발 일정 공유
  - 작성된 명세서에 대한 질의응답 및 개선사항 공유

2. (개인) 기존 api 보완 및 서버 반영

3. (개인) 추가 api 개발
   - 쿠폰 조회
   - 공지 사항
   - 영수증 
   
4. 약관 , 개인정보 정책 등에 필요한 추가 테이블 구성
   
### 2022-02-07 (11일차)

1. (서버)깃허브 브랜치 2차 병합
   - 병합과정에서 오류가 발생해 2월 9일로 일정 지연
   - 계속 오류가 발생할 시 저번처럼 수작업으로 진행

2. (서버)prod 데이터베이스 채우기 작업 진행
   - 데이터의 통일성을 위해 형식 통일
   
3. (개인)지금까지 개발했던 api에 대해 명세서 작성 , 서버 반영

### 2022-02-08 (12일차)

1. (서버)깃허브 브런치 병합 
   - 병합 후 api 테스트 진행 , 오류 사항 수정
   
2. (서버)영수증 api 구현
   - 가게 , 주소 , 가격 , 메뉴 , 옵션들이 나오도록 설정
   - 서버 반영 완료
   
3. (서버)prod db 작업 일정 공유 

4. (서버)최종 배포 일자 논의
   - 2/9 오후 4시로 결정

### 2022-02-09 (13일차)

1. prod 서버로 최종 배포

2. prod 서버에 https 적용
   - 9000번 포트는 이미 사용중이므로 https 리다이렉션 적용
   
3. api 리턴값 변경

4. prod 서버어 바뀜에 따라 api명세서 url 변경 및 샘플 수정









