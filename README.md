# 🧀 카페 급여 및 근무 일정 관리 서비스 | 우아한 치즈케잌

<img width="1200" height="240" alt="woochee logo" src="https://github.com/user-attachments/assets/c5e5bef5-7914-4218-ae21-84d0dee7a9f8" />

## 🗂️ 프로젝트 소개

> `우아한 치즈케잌`은 아르바이트 스케줄이 자주 변경되는 카페 환경에서 근무 누락과 급여 불투명성 문제를 해결하고자 시작된 급여 및 근무 일정 관리 서비스입니다.

## 🗓️ 프로젝트 기간

| 종류 | 기간 |
| :--- | :--- |
| 기획 및 설계 | 2024. 07. 22. ~ 2024. 07. 24. |
| 디자인 | 2024. 07. 25. ~ 2024. 08. 04. |
| 퍼블리싱 및 기능 구현 | 2024. 07. 29. ~ 2024. 08. 08. |

## 🔗 배포 링크

### [🧀 우아한 치즈케잌](https://woowahan-siblings.web.app)

#### 👤 테스트 계정

-   ID : `woochee`
-   PW : `woochee123`

## 📚 기술 스택

| 기술 | 도입 이유 |
| :--- | :--- |
| `React` | 프로젝트에서 사용되는 UI 요소를 독립적이고 재사용 가능한 컴포넌트 단위로 개발하여, 애플리케이션의 유지보수성과 재사용성을 높이기 위해 도입되었습니다. |
| `TypeScript` | 코드에 타입을 명시하여 개발 단계에서 오류를 미리 잡고, 변수나 함수의 의도를 명확하게 만들어 코드의 안정성과 협업 효율성을 높이기 위해 도입되었습니다. |
| `Redux` | 사용자 정보, 근무 일정과 같은 애플리케이션 내의 여러 컴포넌트가 공유해야 하는 전역 클라이언트 상태를 체계적으로 관리하기 위해 도입되었습니다. |
| `React Query` | API 데이터 로딩, 캐싱, 동기화 등 복잡한 서버 상태 관련 로직을 선언적으로 관리하여 비동기 코드의 복잡도를 낮추고, 서버 데이터 관리를 효율화하기 위해 도입되었습니다. |
| `Emotion` | 스타일을 해당 컴포넌트 파일에 함께 두어 응집도를 높이고, 변수를 활용한 동적 스타일링을 쉽게 구현하여 유지보수성과 개발 편의성을 높이기 위해 도입되었습니다. |
| `Firebase` | 별도의 백엔드 서버를 직접 구축하고 배포하는 대신, Firebase가 제공하는 인증 및 데이터베이스를 활용하여 핵심 기능 구현에 집중하기 위해 도입되었습니다. |
| `Vite` | 빠른 개발 서버 속도와 최적화된 빌드 성능을 통해 개발 경험을 향상시키고, 경로 별칭과 같은 편의 기능을 활용해 생산성을 높이기 위해 도입되었습니다. |
| `Husky`<br/>`lint-staged` | 팀원들이 커밋하기 전에 자동으로 코드 컨벤션을 검사하고 수정하도록 강제하여, 전체 코드베이스의 일관성과 품질을 사람의 개입 없이 높은 수준으로 유지하기 위해 도입되었습니다. |

## ✨ 주요 기능

### 1️⃣ 카페 근무 스케줄 관리

#### ◼️ 공식 스케줄 조회

- 카페의 공식 근무 스케줄을 월별 캘린더에서 한눈에 조회할 수 있습니다.

| 공식 스케줄 조회 |
| :---: |
| <img src="https://github.com/user-attachments/assets/4c39b9e0-32e8-44a1-a35e-0bb615552b53" width="300px" alt="schedule view" /> |

#### ◼️ 개인 스케줄 관리(CRUD)

- 공식 스케줄과 별개로, 자신만의 근무 기록용 캘린더를 관리할 수 있습니다.
- 개인 캘린더에 근무 시간, 메모 등을 자유롭게 기록하고 수정 및 삭제할 수 있습니다.

| 개인 스케줄 조회 | 개인 스케줄 추가 | 개인 스케줄 수정 | 개인 스케줄 삭제 |
| :---: | :---: | :---: | :---: |
| <img src="https://github.com/user-attachments/assets/c658b164-f62b-421f-bdd2-1afae47e8020" width="300px" alt="view shift" /> | <img src="https://github.com/user-attachments/assets/66f81824-a2f7-4955-9a1b-014b30d06b3d" width="300px" alt="add shift" /> | <img src="https://github.com/user-attachments/assets/0e63ffdf-911b-4272-8937-1621851b0ab0" width="300px" alt="edit shift" /> | <img src="https://github.com/user-attachments/assets/7187eb33-e40c-4e22-af88-538ae452d2bb" width="300px" alt="delete shift" /> |

### 2️⃣ 근무 및 급여 관리

#### ◼️ 근무 스케줄 기반 급여 조회

- 공식 스케줄 기반의 예상 급여와 개인 기록 기반의 예상 급여를 나란히 비교하여 차이를 쉽게 파악할 수 있습니다.
- 월별 급여 상세 내역(근무 지점, 근무 시간, 시급, 휴게 시간 등)을 확인할 수 있습니다.

| 급여 조회 | 급여 상세 내역 조회 |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/30c71404-bc64-4c63-beb5-30aa1476e11f" width="300px" alt="salary list" /> | <img src="https://github.com/user-attachments/assets/c1bf638c-a40e-4048-aa38-259ac181e390" width="300px" alt="salary detail" /> |

#### ◼️ 근무 정정 신청

- 대타, 특별 근무, 휴가 등 공식 스케줄과 다른 근무가 발생했을 때, 사유와 함께 정정 신청을 제출할 수 있습니다.
- 제출한 정정 신청의 처리 상태(대기, 승인, 반려)를 확인하고 필터링할 수 있습니다.

| 정정 신청 | 정정 신청 내역 조회 | 정정 신청 상세 내역 조회 |
| :---: | :---: | :---: |
| <img src="https://github.com/user-attachments/assets/aaf7aa30-190f-4d44-b495-3522720973d2" width="300px" alt="correction form" /> | <img src="https://github.com/user-attachments/assets/5e62fe7d-59be-426f-897e-5e6c1961bed3" width="300px" alt="correction list" /> | <img src="https://github.com/user-attachments/assets/ae4abaa0-8960-40a0-b77f-1d4eb98b38f1" width="300px" alt="correction detail" /> |

### 3️⃣ Firebase Authentication 기반 사용자 프로필 및 인증

- 아이디와 비밀번호를 통해 안전하게 서비스에 접근하고 로그아웃할 수 있습니다.
- 자신의 이름, 근무 지점, 고정 근무 스케줄 등 개인 정보를 확인할 수 있습니다.

| 로그인 | 사용자 프로필 |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/9c19908f-7f5d-4ea1-ac1b-9f71153b8be4" width="300px" alt="login page" /> | <img src="https://github.com/user-attachments/assets/404b7d96-ef14-41a1-9af4-a2f234f6dd57" width="300px" alt="profile" /> |

## 🤝 협업 방식

### 1️⃣ Git Flow 브랜치 전략

-   `main` : 실제 서비스가 배포되는 안정적인 코드가 병합되는 배포용 브랜치
-   `develop` : 기능 개발이 모두 완료된 코드를 모아 통합하고, 기능별 동작을 확인하는 개발 통합 브랜치
-   `feature/기능명` : 각 기능을 개별적으로 개발하는 기능 브랜치

<img width="800" alt="git flow" src="https://github.com/user-attachments/assets/1cbcb156-7a6b-4195-8ab8-e2234bf5bd87">

### 2️⃣ Slack 채널 내 GitHub 봇 적용

-   GitHub 레포지토리와 Slack의 연동을 통해 새로운 이슈와 작업 상황을 실시간으로 공유해 즉각적인 피드백이 가능했습니다.

<img width="500" src="https://github.com/user-attachments/assets/349f1ac5-46f7-4905-8dbb-20b0334cf7a0" alt="slack github bot" />

## 🧑‍💻 팀원 소개

| 이서윤 | 김대영 | 김동영 | 손성오 | 권혜지 |
| :---: | :---: | :---: | :---: | :---: |
| <img src="https://avatars.githubusercontent.com/u/89791868?v=4" width="150" height="150" alt="seoyoonyi" /> | <img src="https://avatars.githubusercontent.com/u/106634493?v=4" width="150" height="150" alt="dev-meryoung" /> | <img src="https://avatars.githubusercontent.com/u/147500032?v=4" width="150" height="150" alt="love1ace" /> | <img src="https://avatars.githubusercontent.com/u/131119152?v=4" width="150" height="150" alt="Sonseongoh" /> | <img src="https://avatars.githubusercontent.com/u/92978022?v=4" width="150" height="150" alt="hyeppyy" /> |
| [@seoyoonyi](https://github.com/seoyoonyi) | [@dev-meryoung](https://github.com/dev-meryoung) | [@love1ace](https://github.com/love1ace) | [@Sonseongoh](https://github.com/Sonseongoh) | [@hyeppyy](https://github.com/hyeppyy) |

## 🙋‍♂️ 담당 역할 및 기여 내역

### 1️⃣ Firebase Authentication 기반 로그인 기능 구현

-   Firebase를 이용한 로그인/로그아웃 기능 구현 및 세션 관리
-   Redux를 활용한 사용자 정보 전역 상태 관리 및 프로필 페이지 API 연동

### 2️⃣ Firebase Database 기반 API 구현

-   Firebase 연동 및 초기 설정 작업
-   프로젝트 내 모든 API 구현

### 3️⃣ UI/UX 관련 작업

-   로그인 페이지 구현
-   공통 UI 컴포넌트(Input, Button 등) 구현

## 📦 설치 및 실행

### 1️⃣ 설치 과정

#### ◼️ 프로젝트 클론

```
git clone https://github.com/dev-meryoung/woochee.git
cd woochee
```

#### ◼️ 종속성 설치

```
npm install
```

#### ◼️ 환경 변수 설정(.env)

```
VITE_FIREBASE_API_KEY=여기에_발급받은_API_KEY를_입력
VITE_FIREBASE_AUTH_DOMAIN=여기에_발급받은_AUTH_DOMAIN을_입력
VITE_FIREBASE_PROJECT_ID=여기에_발급받은_PROJECT_ID를_입력
VITE_FIREBASE_STORAGE_BUCKET=여기에_발급받은_STORAGE_BUCKET을_입력
VITE_FIREBASE_MESSAGING_SENDER_ID=여기에_발급받은_MESSAGING_SENDER_ID를_입력
VITE_FIREBASE_APP_ID=여기에_발급받은_APP_ID를_입력
VITE_FIREBASE_MEASUREMENT_ID=여기에_발급받은_MEASUREMENT_ID를_입력
```

### 2️⃣ 실행

#### ◼️ 개발 서버 실행

```
npm run dev
```

#### ◼️ 배포용 빌드 실행

```
npm run build
```

## 📁 디렉토리 구조

```
woochee/
├── public/                # index.html에서 직접 참조되는 정적 파일
└── src/                   # 애플리케이션 소스 코드
    ├── api/               # API 요청 함수 (Firebase 연동)
    ├── assets/            # 컴포넌트 내부에서 참조하는 이미지, 아이콘 등
    ├── components/        # 재사용 가능한 공통 UI 컴포넌트
    ├── constants/         # 애플리케이션에서 사용되는 상수
    ├── hooks/             # 공통 로직을 관리하는 커스텀 React 훅
    ├── layout/            # 페이지의 공통 레이아웃 (헤더, 푸터 등)
    ├── pages/             # 라우터에 연결되는 페이지 단위 컴포넌트
    ├── stores/            # Redux Toolkit을 이용한 전역 상태 관리
    ├── styles/            # 전역 스타일, 테마, Reset CSS
    ├── types/             # 공통으로 사용되는 TypeScript 타입 정의
    ├── utils/             # 순수 함수 및 유틸리티 함수
    ├── App.tsx            # 애플리케이션 최상위 컴포넌트 (라우팅 정의)
    ├── firebaseConfig.ts  # Firebase 초기화 및 설정
    └── main.tsx           # 애플리케이션 진입점 (DOM 렌더링)
.
├── .env                   # [추가 필요] Firebase API 키 등 환경 변수 파일
├── .eslintrc.cjs          # ESLint 설정
├── .prettierrc            # Prettier 설정
├── index.html             # 애플리케이션 HTML 템플릿
├── package.json           # 프로젝트 종속성 및 스크립트 관리
└── vite.config.ts         # Vite 설정
```