# Assignment 02

 **학번:** 22500301
 **이름:** 박주아


## Assignment 02 수행 내용

### 1. 각 페이지 설명 및 URL
- **index.html**: 메인 랜딩 페이지. 각 스타일시트 예시 페이지(nostyle.html, style1.html, style2.html)로 이동할 수 있는 네비게이션 링크 제공.
- **nostyle.html**: CSS 스타일이 적용되지 않은 기본 HTML 구조를 보여주는 페이지.
- **style1.html**: Flexbox 레이아웃을 사용하여 상단 헤더, 메인 콘텐츠, 사이드바, 하단 푸터를 녹색/파란색 톤으로 스타일링한 페이지.
- **style2.html**: 내비게이션 메뉴를 가로 형태로 배치하고, 초록색 계열의 제목 스타일을 적용한 페이지.

### 2. Vercel Deploy URL
- **배포 주소:** [https://2026-oss-week2.vercel.app](https://2026-oss-week2.vercel.app)

---

## Weekly Review – Week 2

### 1. Key Learning (이번 주 배운 핵심 내용 3가지)
- **HTML vs CSS:** HTML은 웹페이지의 뼈대와 구조(텍스트, 태그, 디브 등)를 정의하는 언어이고, CSS는 그 뼈대에 색상, 폰트, 레이아웃 등 시각적 스타일을 입히는 언어임을 이해했습니다.
- **Flexbox 레이아웃:** `display: flex` 속성과 `flex-direction`, `gap` 등을 활용하여 요소를 가로/세로로 자유롭게 배치하는 방법을 학습했습니다.
- **외부 CSS 및 이벤트 연결:** HTML 내 `<head>` 태그에서 `<link>`를 이용해 외부 CSS를 연결하는 법과 자바스크립트 함수(`reStyle`)를 통해 특정 링크 클릭 시 페이지 이동을 처리하는 법을 배웠습니다.

### 2. Problem & Solution (실습 중 발생한 문제와 해결 과정)
- **문제:** `<link rel="stylesheet" href="style.css">` 태그를 작성하고 CSS 파일을 생성하여 저장했음에도 브라우저 및 Vercel 배포 페이지에 스타일이 제대로 적용되지 않는 문제가 발생했습니다.
- **해결:** 
  1. `<link>` 태그가 `</head>` 밖에 위치해 있던 오류를 발견하여 `<head>` 내부로 위치를 수정했습니다.
  2. CSS 파일의 수정 사항이 저장(`Cmd + S`)되지 않아 `U` 상태로 남아있던 것을 확인하고 저장했습니다.
  3. Vercel 배포 시 CSS 파일 선택자를 `.container wrapper` (공백 포함)로 잘못 작성했던 오타를 `#top` 등 올바른 선택자로 수정하고, 상대 경로(`./style.css`) 및 파일명 대소문자를 맞춰 다시 `commit` & `push`하여 정상 적용시켰습니다.

### 3. AI Usage (AI 활용 내역)
- **활용 목적:** 외부 CSS 파일 연결 오류 해결, Flexbox 레이아웃 작성 지원, 버튼 클릭 시 외부 링크(`w3schools`)로 이동하는 자바스크립트/HTML 코드 구문 생성에 활용했습니다.


### 4. Reflection (새롭게 알게 된 점 및 궁금한 점)
- **새롭게 알게 된 점:** Vercel과 같은 배포 환경은 리눅스 기반이라 파일명 대소문자나 상대 경로(`./`) 구분에 엄격하다는 점을 알게 되었고, 로컬 테스트와 배포 환경 간의 차이를 점검하는 법을 배웠습니다.여기서 ' ' 되어있는거 다 ' ' 제거해