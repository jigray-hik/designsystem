# HIK Design System ver.1

홈스인코리아 프로덕트의 UI 디자인 시스템입니다.

---

## 색상 시스템

### Main Colors

| 색상 | HEX | 용도 |
|---|---|---|
| Primary Orange | `#FF5C00` | 로고, 버튼, 활성화 상태 |
| Secondary Orange | `#E4661E` | 작은 버튼 (ex. edit), 보조 강조 |

### Background Colors

| 색상 | HEX | 용도 |
|---|---|---|
| Page Bg | `#FFF8F3` | 기본 페이지 배경 |
| Icon Bg | `#F7ECE6` | 아이콘 배경 |
| Sheet/Popup Bg | `#FEFEFE` | Page, 바텀시트, 팝업 배경 |
| Card Text Bg | `#F3F3F3` | 텍스트 카드 배경 (ex. FAQ) |
| Card Bg | `#FFFFFF` | 카드 배경 |
| Overlay | `#000000` 50% | 모달/바텀시트 뒤 오버레이 |
| Shadow | `#666666` 10%, 40% | 그림자 효과 |

### Sub Colors

| 색상 | HEX | 용도 |
|---|---|---|
| Black | `#1F1C1C` | Headline, 강조 텍스트 |
| Warm Black | `#3E2B20` | 기본 본문 텍스트 |
| Warm Brown | `#8B3F11` | 갈색 계열 베리에이션 |
| Gray 1 | `#636262` | 회색 계열 베리에이션 |
| Gray 2 | `#A2A2A2` | 회색 계열 베리에이션 |
| Gray 3 | `#D1D1D1` | 회색 계열 베리에이션 |
| Stroke | `#EFEFEF` | 구분선, 테두리 |

**색상 사용 원칙:**
- 순수한 검정색(`#000000`)을 텍스트에 사용하지 않음 → `#1F1C1C` 사용
- 기본 본문 텍스트는 `#3E2B20` (Warm black)

---

## 폰트

| 폰트 | 용도 | 굵기 |
|---|---|---|
| **Plus Jakarta Sans** | 브랜드, 헤더, Headlines | Extra bold, Bold |
| **Inter** | 주요 UI 폰트 (본문, 라벨, 서브타이틀 전반) | Regular, Bold, Semi bold |

---

## 타이포그래피 시스템 [mobile]

형식: `font / weight / size / line-height`

### Headline
| 토큰 | 폰트 | Weight | Size / LH |
|---|---|---|---|
| headline-lg | Plus Jakarta Sans | Extra bold | 36 / 36 |
| headline-md | Plus Jakarta Sans | Bold | 28 / 28 |
| headline-sm | Plus Jakarta Sans | Bold | 20 / 20 |

### Subtitle
| 토큰 | 폰트 | Weight | Size / LH |
|---|---|---|---|
| subtitle-bold | Inter | Bold | 16 / 16 |
| subtitle-regular | Inter | Regular | 16 / 16 |

### Body
| 토큰 | 폰트 | Weight | Size / LH |
|---|---|---|---|
| body-semi-bold | Inter | Semi bold | 14 / 14 |
| body-regular | Inter | Regular | 14 / 14 |
| body-paragraph | Inter | Regular | 14 / auto |
| md-body-semi-bold | Inter | Semi bold | 13 / 13 |

### Detail
| 토큰 | 폰트 | Weight | Size / LH |
|---|---|---|---|
| detail-semi-bold | Inter | Semi bold | 11 / 11 |
| detail-regular | Inter | Regular | 11 / 11 |
| sm-detail-regular | Inter | Regular | 8 / 8 |

---

## 레이아웃 & 간격

### Spacing Scale (Vertical Rhythm)

섹션 수준의 수직 간격 규칙입니다.

| 용도 | 값 | 설명 |
|---|---|---|
| Between Sections | **48px** | 섹션과 섹션 사이 |
| Text Card / Section Gap | **32px** | 텍스트 카드, 섹션 헤더와 리스트 간 |
| Mixed Card Gap | **24px** | 혼합 카드 리스트 간격 |
| Inline Items | **16px** | 인라인 아이템 간격 |

### Container Margins (Mobile)

- Columns: **4**
- Gutter: **16px**
- Margin (좌우 패딩): **16px**
- Max-width: **360px**

### Container Margins (Responsive)

| 화면 | Viewport | 좌우 Margin | Max-width |
|---|---|---|---|
| Mobile | ~390px | 16px | 390px |
| Tablet | 768 – 1024px | 40px | 100% |
| Desktop | 1024 – 1440px | 40px | 1280px |
| Desktop XL | 1440px 이상 | ~140px | 1280px |

### Border Radius

| 이름 | 값 | 용도 |
|---|---|---|
| None | 0px | 구분선, 풀블리드 요소 |
| Sm | 4px | 태그, 작은 입력 요소 |
| Md | 8px | 버튼, 카드, 일반 컴포넌트 |
| Lg | 24px | 바텀시트, 큰 카드, 모달 |
| Full | 50% | 원형 아이콘 버튼, 칩 |

### Shadows

- **None**: 그림자 없음 (flat)
- 깊이 단계별 shadow 적용
- 고정 버튼 뒤 콘텐츠 스크롤 시: 콘텐츠 `opacity 80%` + `blur 24px`

---

## 컴포넌트

### 기본 컴포넌트

| 컴포넌트 | 설명 |
|---|---|
| **Button** | Primary, Secondary, Tertiary / Button/home type 포함 |
| **Label** | 다양한 상태 (pending, active 등) |
| **Badge** | 숫자/상태 뱃지 |
| **Toggle Switch** | on/off 토글 |
| **Tab** | 탭 네비게이션 |
| **Chips** | 필터/선택 칩 |
| **Search bar** | 검색 입력 바 |
| **Stroke** | 구분선 (`#EFEFEF`) |
| **Input field** | 텍스트 입력 필드 |
| **Progress bar** | 진행 상태 표시 바 |

### 카드 컴포넌트

| 컴포넌트 | 설명 |
|---|---|
| **Mixed Card** | 이미지 + 텍스트 혼합 카드 |
| **Text Card** | 텍스트 기반 카드 (ex. FAQ) |

### 네비게이션

#### [mobile] Header
- **크기**: width 390px × height 65px × 좌우 margin 24px
- **벨 아이콘 규칙**: 새로운 알림이 있을 때만 아이콘 표시

| 타입 | 구성 |
|---|---|
| 기본형 | HOMES 로고 + 벨 아이콘 + 글로브 아이콘 |
| 위시리스트형 | HOMES 로고 + 하트 아이콘 + 글로브 아이콘 |
| 호스트형 | HOMES for host + 벨 아이콘 + 글로브 아이콘 |
| 서브 페이지형 | ＜ 뒤로가기 + 페이지 타이틀 + 벨 아이콘 + 글로브 아이콘 |

#### [mobile] Navigation Bar

| 버전 | 탭 구성 |
|---|---|
| 게스트 | Home / Map / Booking / Chat / My |
| 호스트 | 계약 / 숙소 / 정산 / 메시지 / 마이 |

- 활성 탭: 아이콘 + 텍스트 → `#FF5C00` (Primary Orange)

---

## 로고

### Color Variations
- `#FF5C00` 주황 / `#000000` 검정 / `#FFFFFF` 흰색 3가지 배경 조합

### Primary Logo
- **HOMESINKOREA** 가로형 (주황색)

### Secondary Logo
- **HOMES / INKOREA** 2줄 세로형 (주황색)
- **HOMES** 단독형 (주황색)

---

## 디자인 규칙

### 레이아웃 규칙
- 섹션 구분 시 1px 선 사용 금지 → **배경색 전환**으로 구분
- 섹션 구분선 대신 `#F3F3F3` 또는 `#FFF8F3` 배경 변화 활용

### 색상 규칙
- 텍스트에 `#000000` 사용 금지 → `#1F1C1C` 사용
- 고정 버튼 뒤 스크롤 콘텐츠: opacity 80% + blur 24px

### 네이밍 규칙

**컴포넌트:**
- `Icon/wish`, `Icon/bell off`, `Label/pending`

**페이지:**
- `[HIK]map`, `[HIK]map_view_list`

**유저 상태 구분:**
| 접두사 | 대상 |
|---|---|
| `[HIK_null]` | 비로그인 사용자 (ex. `[HIK_null] my`) |
| `[HIK_guest]` | 게스트 사용자 (ex. `[HIK_guest] my`) |
| `[HIK_host]` | 호스트 사용자 (ex. `[HIK_host] my`) |

---

## 참고

자세한 정보는 [Figma 디자인 시스템](https://www.figma.com/design/7DEB0l3BEOeJWLwbkpxgir/%ED%99%88%EC%8A%A4%EC%9D%B8%EC%BD%94%EB%A6%AC%EC%95%84-%ED%94%84%EB%A1%9C%EB%8D%95%ED%8A%B8?node-id=1939-683)에서 확인해주세요.
