# Portfolio (with Next.js)
Next.js, graphql, typescript ...

<br/><br/>

# Figma 프로토타입 디자인
![image](https://user-images.githubusercontent.com/54789601/214791101-75d0ac8c-acbd-482b-8c61-c8657c29e1f6.png)

<br/><br/>

# 반응형 웹 퍼블리싱
<img width="900" src="https://user-images.githubusercontent.com/54789601/214800581-a2d33148-a3e1-47a0-84e9-f67489557cf9.gif" alt="검색 디바운싱"/>

<br/><br/>

# 글로벌 스타일 코드
![image](https://user-images.githubusercontent.com/54789601/214794706-36590c49-a8ba-4fbf-ae95-8d403a1092f4.png)

<br/><br/>

# 반응형 퍼블리싱 코드 타입
## 1. 전체 스타일드 컴포넌트 스타일링
## 2. 스타일드 컴포넌트와 선택자 조합 스타일링
![image](https://user-images.githubusercontent.com/54789601/214796523-7f99186a-d5c0-467c-96e8-0c5ba46d17d4.png)

<br/><br/>

# 공통 스타일드 컴포넌트 및 재 사용
![image](https://user-images.githubusercontent.com/54789601/214798319-d9988d34-861a-49fc-b904-7aeb87c5d9d8.png)

<br/><br/>

# 검색 디바운싱
- 마지막 입력 기준으로 일정 시간이 지나면 해당 키워드로 한 번만 검색
<img width="900" src="https://user-images.githubusercontent.com/54789601/215017242-025d3e7e-89fd-474c-8f0f-c3d1e2adf543.gif" alt="검색 디바운싱"/>

<br/><br/>

# 무한 스크롤
<img width="900" src="https://user-images.githubusercontent.com/54789601/215017234-56f8d8ae-a5d0-44ef-b85b-764af74c5b29.gif" alt="무한 스크롤"/>

<br/><br/>

# 최적화 
## 프리페치 (데이터 미리 받아오기)
### 프리페치 적용 전
- 페이지 이동 시 데이터를 받아오기 때문에 네트워크가 느린 환경에선 다소 느려보임
<img width="900" src="https://user-images.githubusercontent.com/54789601/215017265-c28630d5-e9f0-455e-b184-15621d114903.gif" alt="프리페치 이전"/>

### 프리페치 적용 후
- 마우스 오버 시 해당 페이지를 들어갈 것이라 가정하고 페이지의 데이터 미리 받아오기 때문에 매우 빠른 UI 출력
<img width="900" src="https://user-images.githubusercontent.com/54789601/215017279-e81e3fcc-4687-43ad-af99-1083c9dfec16.gif" alt="프리페치 이후"/>

<br/><br/>

## 옵티미스틱 UI (낙관적 UI)
- API요청에 대한 결과가 긍정적(성공)일 것이라 기대 하고 결과에 대한 캐시를 미리 업데이트 
- 문제가 생겨도 크리티컬하지 않은 서비스에 적용 ( 구독 또는 좋아요 )

### 옵티미스틱 UI 적용 전
- 요청 후 업데이트 된 값을 반영하기 때문에 네트워크가 느린 환경에선 다소 느려보임
<img width="900" src="https://user-images.githubusercontent.com/54789601/215028617-51836976-ba20-4d3b-af03-e3e0c92ed087.gif" alt="XSS 공격 방지 처리 전"/>

### 옵티미스틱 UI 적용 후
- 요청과 동시에 캐시 값을 직접 수정하기 때문에 반응이 매우 빠르게 보임
<img width="900" src="https://user-images.githubusercontent.com/54789601/215028624-8f245d04-8e9f-4506-990d-d1785e9611a4.gif" alt="XSS 공격 방지 처리 전"/>

<br/><br/>

# XSS 공격 방지 (dompurify) - Text Editor 라이브러리 사용 시 스크립트 문자 처리
- 임의로 스크립트로 작성 된 게시글을 등록 
- 실제 백 엔드 XSS관련 처리 로직이 제대로 동작하지 않았을 모든 상황을 가정

## XSS 공격 방지 처리 전
- 해당 페이지 접근 시 스크립트 실행
<img width="900" src="https://user-images.githubusercontent.com/54789601/215020518-df5f3982-7189-4d9b-9193-818f5a233775.gif" alt="XSS 공격 방지 처리 전"/>

## XSS 공격 방지 처리 후
- 해당 페이지 접근 시 스크립트 실행하지 않음
<img width="900" src="https://user-images.githubusercontent.com/54789601/215020408-b6238bd6-c11c-41bb-948c-f1febea6351e.gif" alt="XSS 공격 방지 처리 후"/>



