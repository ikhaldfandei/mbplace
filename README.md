# 마케팅 허브 (Marketing Hub)

개인 병원 마케팅 업무 통합 관리 툴

## 📦 GitHub Pages 배포 방법 (5분 설정)

### 1단계: 저장소 만들기
1. [github.com](https://github.com) 로그인
2. 우측 상단 `+` → **New repository**
3. Repository name: `marketing-hub` (원하는 이름)
4. **Public** 선택 (Pages 무료 사용 조건)
5. **Create repository** 클릭

### 2단계: 파일 업로드
1. 방금 만든 저장소 페이지에서 **uploading an existing file** 클릭
2. `index.html` 파일을 드래그 앤 드롭
3. **Commit changes** 클릭

### 3단계: GitHub Pages 활성화
1. 저장소 상단 **Settings** 탭
2. 왼쪽 메뉴 **Pages** 클릭
3. Source → **Deploy from a branch**
4. Branch → **main** 선택 → `/ (root)` → **Save**
5. 약 1분 후 `https://[내아이디].github.io/marketing-hub/` URL 생성됨

### 4단계: GitHub 동기화 토큰 만들기
1. GitHub 우측 상단 프로필 → **Settings**
2. 맨 아래 **Developer settings** → **Personal access tokens** → **Tokens (classic)**
3. **Generate new token (classic)**
4. Note: `마케팅허브 동기화`
5. Expiration: `No expiration` (또는 1년)
6. 권한 체크: ✅ **gist** 만 체크
7. **Generate token** → 나온 토큰 복사 (다시 볼 수 없음!)

### 5단계: 앱에서 토큰 등록
1. 생성된 URL 접속
2. 비밀번호 설정 (첫 실행 시 자동 설정)
3. **설정** 탭 → **GitHub 동기화** 섹션
4. GitHub 토큰 입력
5. **☁️ ↑ GitHub에 저장** 버튼 클릭 → 첫 저장 시 Gist 자동 생성

### 6단계: 다른 PC에서 연결
1. 같은 URL 접속
2. **설정** → **GitHub 동기화** → 토큰 입력
3. **☁️ ↓ GitHub에서 불러오기** 클릭 → 완료!

---

## 🔄 일상적인 사용법

| 상황 | 할 일 |
|---|---|
| 회사에서 작업 완료 후 집 갈 때 | **☁️ ↑ GitHub에 저장** 클릭 |
| 집에서 열었을 때 | **☁️ ↓ GitHub에서 불러오기** 클릭 |
| 평소에는 | 그냥 쓰면 됨 (자동 로컬 저장) |

---

## ⚙️ 기능 목록

- 📝 **클라이언트 노트**: 트리 구조, 드래그 순서 변경, 분할 보기
- 🗂 **업무 노트**: 개인전략, AI프롬프트, 매뉴얼, 상사 전달사항 등
- 📅 **월간 스케줄**: 엑셀 형태 스케줄 + 잔여 횟수 트래커 (리사이즈 가능)
- 📁 **월간 보고서**: PDF/PPTX 파일 업로드 및 관리
- ☁️ **GitHub 동기화**: 집/회사 어디서든 동일한 데이터

