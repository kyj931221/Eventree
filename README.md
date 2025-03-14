# 이벤트리(Eventree) 앱 기획서 및 개발 과정

## 1. 기획서

### 1.1. 서비스 개요
- **서비스명:** 이벤트리(Eventree)
- **서비스 목표:** 다양한 이벤트를 위한 맞춤형 콘텐츠 생성 및 공유 서비스 제공
- **타겟 사용자:** 특별한 순간을 기념하고 공유하고자 하는 모든 사용자
- **주요 기능:**
  - 다양한 이벤트 템플릿 제공 (임신 소식, 생일, 기념일 등)
  - 사용자 맞춤형 콘텐츠 생성 (텍스트, 이미지, 멀티미디어)
  - 생성된 콘텐츠의 HTML 형식 다운로드 및 공유 기능
  - 각 이벤트에 맞는 특수효과 및 애니메이션 제공

### 1.2. 초기 서비스: 임신 소식 알림 서비스
- **주요 기능:**
  - 임신 소식 관련 정보 입력 (날짜, 성별, 태명, 이미지, 문구)
  - 입력된 정보를 기반으로 디자인된 HTML 페이지 자동 생성
  - 성별에 따른 맞춤형 시각 효과 (색상, 애니메이션)
  - 생성된 페이지의 다운로드 및 공유 기능

### 1.3. 화면 구성
- **메인 시작 화면:**
  - 앱 로고 및 간단한 소개 문구
  - "서비스 시작" 버튼
- **이벤트 리스트 화면:**
  - 다양한 이벤트 목록 (스크롤 뷰)
  - 각 이벤트별 간단한 소개 및 미리보기
  - 이벤트 선택 시 해당 서비스 화면으로 이동
- **이벤트 서비스 화면 (임신 소식 알림):**
  - 날짜 선택 (DatePicker)
  - 성별 선택 (남/여/쌍둥이, 복수 선택 가능)
  - 태명/이름 입력 (TextInput, 복수 입력 가능)
  - 이미지 등록 (Image Picker)
  - 안내 문구 입력 (TextInput)
  - 생성 버튼
- **결과 화면:**
  - 생성된 HTML 페이지 미리보기
  - 성별에 따른 시각 효과 및 애니메이션
  - 다운로드 및 공유 버튼

### 1.4. 기술 스택
- Unity 6: 앱 개발 플랫폼
- HTML, CSS, JavaScript: 웹 페이지 생성 및 디자인
- C#: Unity 스크립트 언어
- Firebase 또는 AWS: 데이터 저장 및 관리 (선택 사항)

## 2. 개발 과정

### 2.1. 프로젝트 설정
- Unity 6 프로젝트 생성
- 필요한 에셋 및 플러그인 설치 (UI, 이미지 처리, 웹뷰 등)
- 프로젝트 구조 설계 (씬, 스크립트, 에셋 관리)

### 2.2. UI 디자인 및 구현
- 각 화면별 UI 디자인 (Unity UI Canvas)
- 사용자 입력 요소 구현 (InputField, Toggle, DatePicker 등)
- 이벤트 리스트 및 결과 화면 디자인 (ScrollView, WebView)
- 성별에 따른 시각 효과 및 애니메이션 구현 (Particle System, Animator)

### 2.3. 기능 구현
- 사용자 입력 데이터 처리 및 저장 (C# 스크립트)
- HTML 페이지 템플릿 생성 및 데이터 바인딩
- 웹 페이지 생성 및 미리보기 (WebView)
- 다운로드 및 공유 기능 구현 (Native Share, File I/O)
- 성별에 따른 맞춤형 시각 효과 및 애니메이션 적용

### 2.4. 테스트 및 디버깅
- 각 기능별 단위 테스트 및 통합 테스트
- 다양한 기기 및 환경에서의 테스트
- 버그 수정 및 성능 개선

### 2.5. 배포
- Android 및 iOS 빌드 설정
- 각 앱 스토어에 앱 등록 및 배포
- 사용자 피드백 수렴 및 지속적인 업데이트

## 3. 추가 고려 사항
- 사용자 경험 (UX): 직관적이고 사용하기 쉬운 UI/UX 디자인
- 성능 최적화: 다양한 기기에서 원활하게 작동하도록 최적화
- 보안: 사용자 데이터 보호 및 보안 강화
- 다국어 지원: 글로벌 사용자 확보를 위한 다국어 지원
- 소셜 미디어 연동: 공유 기능 강화 및 사용자 참여 유도
- 데이터 분석: 사용자 행동 분석을 통한 서비스 개선
