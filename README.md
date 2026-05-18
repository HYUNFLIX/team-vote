# 우수팀 투표 (Team Vote)

QR코드 기반 실시간 우수팀 투표 앱

**Live**: https://hyunflix.github.io/team-vote/

## 사용법

### 관리자
1. 사이트 접속 → **관리자 설정**
2. 과제명 + 팀 이름 입력 → **저장 및 시작**
3. QR코드 또는 6자리 참여 코드를 학습자에게 공유
4. **결과 보기**로 실시간 집계 확인

### 학습자
1. QR코드 스캔 또는 참여 코드 입력
2. 팀 선택 → 투표 (1인 1표)

## 기술 스택
- **Frontend**: HTML + Tailwind CSS + Vanilla JS (단일 파일)
- **Backend**: Firebase Realtime Database
- **배포**: GitHub Pages
- **폰트**: Noto Sans KR, Black Han Sans (Google Fonts)
- **QR**: qrserver.com API

## 프로젝트 구조
```
├── index.html              # 앱 전체 (HTML+CSS+JS)
├── database.rules.json     # Firebase DB 보안 규칙
├── README.md               # 프로젝트 소개
├── DESIGN.md               # 디자인 시스템 문서
├── TODO.md                 # 개발 로드맵
└── .github/
    └── workflows/
        └── deploy.yml      # GitHub Pages 자동 배포
```
