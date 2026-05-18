# 우수팀 투표 (Team Vote)

QR코드 기반 실시간 우수팀 투표 앱

**Live**: https://hyunflix.github.io/team-vote/

## 사용법

### 관리자
1. [관리자 페이지](admin.html) 접속
2. 과제명 + 팀 이름 입력 → **저장 및 시작**
3. QR코드 또는 6자리 참여 코드를 학습자에게 공유
4. **투표 마감** → **순위 공개** → **프로젝터 모드**

### 학습자
1. QR코드 스캔 또는 메인 페이지에서 참여 코드 입력
2. 팀 선택 → 투표 (1인 1표)

## 기술 스택
- **Frontend**: HTML + Tailwind CSS + Vanilla JS
- **Backend**: Firebase Realtime Database
- **배포**: GitHub Pages
- **폰트**: Noto Sans KR (Google Fonts)
- **QR**: qrserver.com API
- **디자인**: Apple HIG / iOS 금융 앱 스타일

## 프로젝트 구조
```
├── index.html              # 투표자 페이지 (홈 + 투표)
├── admin.html              # 관리자 페이지 (설정 + QR + 결과)
├── database.rules.json     # Firebase DB 보안 규칙
├── README.md               # 프로젝트 소개
├── DESIGN.md               # 디자인 시스템 문서
├── TODO.md                 # 개발 로드맵
└── .github/
    └── workflows/
        └── deploy.yml      # GitHub Pages 자동 배포
```
