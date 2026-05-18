# 디자인 시스템

## 브랜드 컬러
| 용도 | 컬러 | HEX |
|------|------|-----|
| Primary | Indigo | #6366f1 |
| Primary Dark | Violet | #8b5cf6 |
| Accent | Purple | #a855f7 |
| Background | Slate 50 | #f8fafc |
| Text Primary | Slate 800 | #1e293b |
| Text Secondary | Slate 400 | #94a3b8 |

## 팀 카드 그라데이션 (8색 순환)
| # | 이름 | 시작 → 끝 | 이모지 |
|---|------|-----------|--------|
| 1 | Pink | #f472b6 → #ec4899 | :pink_heart: |
| 2 | Blue | #38bdf8 → #3b82f6 | :blue_heart: |
| 3 | Green | #34d399 → #10b981 | :green_heart: |
| 4 | Orange | #fb923c → #f97316 | :orange_heart: |
| 5 | Violet | #a78bfa → #8b5cf6 | :purple_heart: |
| 6 | Red | #f87171 → #ef4444 | :heart: |
| 7 | Teal | #2dd4bf → #14b8a6 | :light_blue_heart: |
| 8 | Amber | #fbbf24 → #f59e0b | :yellow_heart: |

## 타이포그래피
| 용도 | 폰트 | 굵기 |
|------|------|------|
| 제목/우승팀 | Black Han Sans | 400 |
| 본문 | Noto Sans KR | 300~900 |
| 코드/Config | monospace (시스템) | - |

## 컴포넌트
### 버튼
- **Primary**: gradient indigo→violet, 라운드 2xl, hover시 그림자 확대
- **Glass**: 반투명 흰색 배경 + blur, 흰색 테두리
- **Disabled**: slate-200 배경, slate-400 텍스트

### 카드
- 흰색 배경, 라운드 2xl, 미세 그림자 + slate-100 보더
- 팀 카드: 그라데이션 배경, 선택시 ring-4 white + scale 1.04

### 애니메이션
| 이름 | 효과 | 지속시간 |
|------|------|----------|
| fadeInUp | 아래→위 + 투명→불투명 | 0.6s ease-out |
| slideIn | 왼→오 + 투명→불투명 | 0.5s ease-out |
| float | 위아래 떠다님 | 3s infinite |
| pulseGlow | 박스 그림자 펄스 | 2s infinite |
| shimmer | 텍스트 금빛 반짝임 | 3s linear infinite |
| bar-fill | 막대 너비 확장 | 1.8s cubic-bezier |

## 페이지 구성 (5+1)
```
홈 ──→ 관리자 설정 ──→ QR/대기 ──→ 결과
          │                              ↑
          └── Firebase 설정 (최초 1회)    │
                                         │
홈 ──→ 투표 참여 (QR/코드) ─────────────┘
```

## 반응형
- 모바일 퍼스트 (max-w-lg 컨테이너)
- 홈 버튼: 모바일 세로 → 데스크탑 가로 (sm:flex-row)
- user-scalable=no (투표 앱 특성상 확대 불필요)
