# [프론트엔드 개발자] 최서아
## AI 서비스개발 프로젝트 구축 기술스택

Fol:in 클론코딩

**`[소개]`**

각 직군 전문가의 경험을 바탕으로 한 콘텐츠 구독 서비스입니다. ([folin 공식링크](https://www.folin.co/)) 프론트엔드 개발을 중심으로 백엔드, DB구성, CI/CD 전체적인 작업을 진행하였습니다.

**`[기간]`**

- 2025.06.09 ~ 2025.07.04 (이후 계속 작업 중)
- 메인: 8일, 서브4장: 7일 , 백엔드: 5일 정도 소요

**`[인원]`**

1명

**`[개발 내용]`**

프론트엔드
- Nextjs 프레임워크 사용, 서버/클라이언트 컴포넌트 분리 구조, 페이지 기반 라우팅 초기 데이터 렌더링 최적화
- Tailwind CSS로 반응형, 여백, 색상 스타일링 처리
- next/image 를 활용해 이미지 최적화 및 lazy loading 적용
- Metadata API활용 설명(description), 키워드(keywords) 등을 세분화해 설정함으로써 검색 엔진에서의 가독성과 노출률 향상
- Series별 Color Mapping createColorAssigner()로 시리즈마다 고유 색상 매핑

백엔드
- express 프레임워크
- dotenv: 환경변수 관리, nodemon: 변경 사항 바로 반영 가능하므로 디버깅 속도 향상
- morgan: 요청 정보 보기, cors: 교차출처요청 관리
- mysql, 워크벤치로 데이터베이스 정규화하여 구성

Open AI 챗봇
- 파이썬기반 fastapi 프레임워크
- Open AI api 활용, 모델: gpt-4.1-mini

CI, CD
- 프로젝트별 깃허브 레포지토리에 통합
- 프론트는 버셀 클라우드에 배포
- express 백엔드는 도커기반 깃헙액션 이용한 aws EC2 빌드, 배포
- DB는 aws RDS에 워크벤치 ssh접속하여 구성
- fastapi는 도커기반 깃헙액션 이용한 aws EC2에 서비스 추가하여 빌드, 배포

**`[Github 링크]`**

[폴인프론트엔드](https://github.com/seoa-choi/folin-frontend.git)
[폴인백엔드](https://github.com/seoa-choi/folin-backend.git)
[fastapi-chatgpt](https://github.com/seoa-choi/fastapi-chatgpt.git)

**`[프로젝트 링크]`**

[https://seoachoiaws.com](https://seoachoiaws.com)
