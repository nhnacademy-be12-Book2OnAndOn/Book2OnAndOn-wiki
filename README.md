# Book2OnAndOn Team wiki

## 팀 협업 규칙 (Team Wiki)

원활한 프로젝트 진행을 위해 다음 규칙을 준수합니다.

### 1. 회의
* **데일리 스크럼 (Daily Scrum)**
    * **시간:** 매일 오전 9시 (약 15분)
    * **방식:** 대면 회의 (필참)
    * **공유 내용 (3가지):**
        1.  어제 한 일 (Done)
        2.  오늘 할 일 (To-Do)
        3.  문제점 / 공유사항 (Blocker / Issues)
* **정기 주간 회의**
    * **시간:** 매주 금요일 오후 4시 (약 1시간)
    * **내용:** 한 주간 진행 상황 요약, KPT(Keep-Problem-Try) 회고, 다음 주 계획 수립

### 2. Git 컨벤션
* **브랜치 전략 (Git-Flow 변형)**
    * `main`: 최종 배포 브랜치 (안정)
    * `develop`: 개발 메인 브랜치 (다음 배포 버전)
    * `feature/[기능명]`: 기능 개발 브랜치 (예: `feature/cart`)
        * `develop` 브랜치에서 분기합니다.
        * 개발 완료 시 `develop` 브랜치로 Pull Request (PR)
    * `fix/[이슈명]`: 긴급 버그 수정 브랜치
* **커밋 메시지 (Commit Message)**
    * 형식: `[Type]: [Subject]` (예: `Feat: 장바구니 추가 기능 구현`)
    * **Types:**
        * `Feat`: 새로운 기능 추가
        * `Fix`: 버그 수정
        * `Docs`: 문서 수정
        * `Style`: 코드 스타일 변경 (포맷팅, 세미콜론 등)
        * `Refactor`: 코드 리팩토링
        * `Test`: 테스트 코드 추가/수정
        * `Chore`: 빌드 설정, 패키지 매니저 관리 등

### 3. 코딩 컨벤션
* **스타일:** Google Java Style Guide 준수
* **네이밍 (Java):**
    * 클래스: `UpperCamelCase` (예: `BookService`)
    * 메서드/변수: `lowerCamelCase` (예: `addToCart`)
    * 상수: `ALL_CAPS_SNAKE_CASE` (예: `MAX_STOCK_COUNT`)
* **네이밍 (DB):**
    * 테이블/컬럼: `snake_case` (예: `cart_item`, `member_id`)

### 4. 이슈 관리 (GitHub Issues)
* **템플릿:** 기능 개발(`Feature`), 버그 리포트(`Bug`) 템플릿 사용
* **라벨:** `Backend`, `Frontend`, `Bug`, `High-Priority` 등 라벨을 적극 활용하여 이슈 분류
