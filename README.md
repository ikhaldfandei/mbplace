# 📋 MBHub — 마케팅 허브

> 병원 마케팅 실무자를 위한 올인원 업무 관리 툴  
> Google Drive 연동 · PC + 모바일 완전 지원 · 서버 불필요

---

## ✨ 주요 기능

| 탭 | 기능 |
|---|---|
| 📝 **클라이언트** | 담당 업체별 문서·메모·회의록 관리, 폴더 트리, 분할 편집 |
| 🗂 **통합문서** | 클라이언트 무관 공용 메모 · 전략 노트 |
| 📅 **스케줄** | 월간 콘텐츠 스케줄 표, 채널별 트래커, 주간 업무 요약 자동 생성 |
| 📁 **보고서** | 클라이언트별 보고서 파일 업로드 · Drive 자동 동기화 |
| 📖 **출판** | 텀블벅 / 출판사 정산 / 집필 파일 통합 관리 |
| ⚙️ **설정** | 클라이언트 관리, Google Drive 연동, 알림, 테마 |

---

## 🚀 빠른 시작

### 1. GitHub Pages 배포

```
1. 이 저장소를 Fork 하거나, 새 저장소를 만들고 index.html 업로드
2. Settings → Pages → Source: Deploy from a branch → main / (root) → Save
3. 배포 URL: https://[GitHub아이디].github.io/[저장소명]/
```

### 2. Google Drive 연동 설정

```
1. console.cloud.google.com → 새 프로젝트 생성
2. API 및 서비스 → OAuth 동의 화면 설정
3. 사용자 인증 정보 → OAuth 클라이언트 ID 생성 (웹 애플리케이션)
4. 승인된 JavaScript 원본: https://[GitHub아이디].github.io
5. 승인된 리디렉션 URI: https://[GitHub아이디].github.io/[저장소명]/
6. Google Drive API 사용 설정
7. 발급된 클라이언트 ID를 앱 설정 탭에 입력
```

### 3. 첫 실행

```
1. 배포 URL 접속
2. 설정 탭 → Google Drive 연동 → 클라이언트 ID 입력 → Drive 연결
3. 설정 탭 → 클라이언트 관리 → 담당 업체 추가
4. 설정 탭 → 알림 설정 → 브라우저 알림 권한 허용
```

---

## 📦 기술 스택

- **프론트엔드**: Vanilla JS · HTML · CSS (프레임워크 없음)
- **스토리지**: IndexedDB (로컬) + Google Drive (클라우드)
- **인증**: Google Identity Services (GIS) — 서버 불필요
- **에디터**: 커스텀 contentEditable 기반 리치 에디터
- **배포**: GitHub Pages (정적 호스팅)

---

## 🗂 파일 구조

```
index.html        ← 앱 전체 (단일 파일)
README.md         ← 이 문서
```

> 모든 코드가 `index.html` 하나에 포함되어 있습니다.  
> 업데이트 시 `index.html`만 교체하면 됩니다.

---

## 💾 데이터 저장 방식

```
로컬 저장     IndexedDB  → 브라우저를 닫아도 유지
클라우드 저장  Google Drive → 수동 저장 (Ctrl+S) 또는 자동 저장
기기 간 동기화 Drive ↑저장 → 다른 기기에서 ↓불러오기
```

> 데이터는 사용자의 Google Drive에만 저장됩니다.  
> 외부 서버로 전송되는 데이터 없음.

---

## ⌨️ 주요 단축키

| 단축키 | 기능 |
|---|---|
| `Ctrl+S` | Google Drive 저장 |
| `Ctrl+K` | 전체 검색 |
| `Ctrl+B` | 굵게 |
| `Ctrl+I` | 기울임 |
| `Tab` (스케줄) | 오른쪽 셀 이동 |
| `Ctrl+클릭` (스케줄) | 셀 다중 선택 |

---

## 📱 모바일 지원

- 아이패드 / 스마트폰 완전 지원
- 하단 탭바로 탭 전환
- ☰ 버튼으로 사이드바 드로어 열기
- 마지막 열람 상태 기기별 자동 복원

---

## 📄 라이선스

개인 사용 목적으로 자유롭게 사용 가능합니다.
