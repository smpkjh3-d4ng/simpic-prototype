# component.md — Simpic 컴포넌트 목록과 사용법

> DESIGN.md의 Components 섹션이 가리키는 문서예요. 컴포넌트 이름·variant·속성과 쓰는 법을 적어요.
> 출처: Figma `디자인md 수정` 페이지 › `Components(수정용)` 섹션 (node 1580:955). 각 컴포넌트의 설명(description)과 속성(component properties)을 그대로 옮겼어요. (2026-11-16 기준)
> Figma 컴포넌트는 2026-11-14 기준이에요. 그 뒤 GitHub 최신 프로토타입(2026-11-16)에서 바뀐 점은 각 항목과 맨 아래 표에 함께 적었어요.
> **카테고리 이름:** Figma variant 값의 `덕질`은 지금 앱에서 **취미**예요(2026-11-16 변경). 코드와 문서에서는 취미로 불러요.
> 값(색·글자·간격·모서리·그림자)은 DESIGN.md의 토큰 이름으로만 적어요. 이 문서와 DESIGN.md가 다르면 **DESIGN.md(최종 프로토타입 기준)를 따라요.** 서로 다른 곳은 맨 아래 "Figma와 DESIGN.md가 다른 곳"에 모았어요.

## 읽는 법

- **속성 표기:** `이름(V)` variant, `이름(T)` 글자, `이름(B)` 켜고 끄기, `이름(Swap)` 아이콘 바꾸기. 괄호 안 값은 Figma 기본값이에요.
- **상태(State):** 버튼·칩은 Default · Pressed · Disabled(· Loading)를 모두 그려 둬요. Focus는 따로 그리지 않고 기기 기본 표시를 써요.
- **[다크 예외]:** 사진 상세·베스트컷 만들기처럼 DESIGN.md "예외 — 다크 화면"을 따르는 컴포넌트예요. 흰색 계열(`dark.white-alpha-*`)을 써요.
- 컴포넌트 이름 끝의 `(수정용)`은 Figma 작업용 표시예요. 코드와 문서에서는 빼고 불러요(예: `Chip`).

## 목록

| 묶음 | 컴포넌트 | Variant 수 | Figma ID |
|---|---|---|---|
| 공통 | Header | 5 | 1580:1076 |
| 공통 | Icon Button | 15 | 1580:1099 |
| 공통 | Text Button | 2 | 1580:1130 |
| 공통 | Section Title | — | 1580:20631 |
| 공통 | Status Bar | 2 | 1580:1136 |
| 공통 | Navigation Bar | 2 | 1580:1141 |
| 공통 | Icons (Icon/*) | — | 1580:1029 |
| 공통 | Icon/bestcut | 3 | 1580:1043 |
| 공통 | Icon/like | 3 | 1580:1065 |
| 공통 | Chip | 9 | 1580:1149 |
| 공통 | Button / Primary | 4 | 1580:1177 |
| 공통 | Button / Bottom | 11 | 1580:1197 |
| 공통 | 구분선 (Divider) | 2 | 1580:1004 |
| 공통 | Hint Card | — | 1580:20570 |
| 홈 | Logo | — | 1580:20576 |
| 홈 | Profile Button | — | 1580:20573 |
| 홈 | Tab Bar | 2 | 1580:1013 |
| 홈 | Album Card | 3 | 1580:1255 |
| 홈 | Avatar Stack | 3 | 1580:1234 |
| 홈 | Group Row | — | 1580:20622 |
| 친구 | Friend Row | — | 1585:2861 |
| 친구 | Group Row / 친구 탭 | — | 1585:2869 |
| 앨범 상세 | Album Hero | 3 | 1580:963 |
| 앨범 상세 | 앨범 상단 · 친목 | — | 1612:2281 |
| 앨범 상세 | 앨범 필터 줄 (템플릿, 컴포넌트 아님) | — | 1612:2284 |
| 앨범 상세 | Stats Card | — | 1580:20606 |
| 앨범 상세 | Top 3 Stack | — | 1580:20590 |
| 앨범 상세 | Photo Thumbnail | — | 1580:20592 |
| 앨범 상세 | 사진 그리드 (Photo Grid) | — | 1580:20584 |
| 사진 상세 | Comment Chip [다크 예외] | 3 | 1580:1301 |
| 사진 상세 | Action Bar Item [다크 예외] | — | 1580:20540 |
| 베스트컷 만들기 | Blurred Background [다크 예외] | — | 1580:20543 |
| 베스트컷 만들기 | Photo Canvas | — | 1580:20546 |
| 베스트컷 만들기 | Prompt Input [다크 예외] | — | 1580:20562 |
| 색 견본 | 색 · Success · Danger · 카테고리 팔레트 (프레임) | — | 1640:3022 |

---

## 공통

### Header
- **속성:** `Type(V)` Home | Album | Dark | Dark Date | Back · `Title(T)` ("베스트컷 만들기") · `Date(T)` ("10월 4일 오후 1:05 · 서연")
- **모양:** 412×44, 좌우 `page-margin`, 상태바 바로 아래(사이 0).
- **Type별 쓰는 곳**
  - Home: 로고 + 검색·프로필 (홈)
  - Album: 뒤로 + 더보기 유리 버튼 (앨범 상세). 스크롤하면 앨범 이름이 뒤로 버튼 옆에 왼쪽 정렬로 나오고 버튼은 아이콘만 남아요.
  - Dark: 닫기 + 가운데 제목 + 보정 기록·'저장' (베스트컷 만들기)
  - Dark Date: 닫기 + 제목(`body-md`)·날짜(`body-sm`) 두 줄 왼쪽 정렬 + 더보기 (사진 상세)
  - Back: 뒤로(Surface) + 가운데 제목 + 오른쪽 빈 자리 (내 프로필·문서 스캔 같은 밝은 단계 화면)
- **규칙:** 제목은 화면 정가운데(Dark Date만 예외). 상단 버튼은 44×44, 사이 8 (`sm`).

### Icon Button
- **속성:** `Style(V)` Surface | Translucent | Glass | Ghost · `Size(V)` 44 | 40 · `State(V)` Default | Pressed | Disabled · `Icon(Swap)`
- **Style별 쓰는 곳:** Surface=흰 바탕 위 · Translucent=사진·그라데이션 위(44는 그림자, 40은 없음) · Glass=다크 유리 · Ghost=다크 화면의 바탕 없는 버튼(보정 기록)
- **Size:** 44 기본, 40은 앨범 필터 줄에만.
- **상태:** 밝은 면 Pressed=바탕 `border`, Disabled=아이콘 `disabled`. Glass Pressed=바탕 `white-alpha-40`, Disabled=아이콘 `white-alpha-40`. Ghost Pressed=바탕 `white-alpha-20`.
- **접근성:** 아이콘만 있는 버튼이라 이름(aria-label)이 꼭 필요해요(예: '친구 메뉴 더보기'). 40 크기도 누르는 영역은 48로 넓혀요.

### Text Button
- **속성:** `Style(V)` Translucent | Dark Ghost · `Label(T)` ("선택")
- **모양:** 높이 44 알약. Translucent=사진·그라데이션 위(`body-md`, `surface-translucent`). Dark Ghost=다크 화면의 비활성 글자 버튼(베스트컷 '저장', `label-md`, `white-alpha-40`).

### Section Title
- 섹션 제목(`headline-md`) + 더보기 링크(`body-sm`, `secondary`). 제목 → 내용 12 (`md`), 섹션 사이 32 (`2xl`).

### Status Bar · Navigation Bar
- **속성:** `Theme(V)` Light | Dark
- Status Bar: 갤럭시(One UI) 상태바 412×44. 삼성 UI 키트 인스턴스를 감싼 것이라 시간·배터리 같은 세부 값은 안쪽 인스턴스에서 바꿔요.
- Navigation Bar: 삼성 3버튼 내비게이션 412×48, 모든 화면 맨 아래.
- 키트 안의 값(안쪽 여백 15 등)은 토큰이 아닌 시스템 UI 예외예요. 다크 화면은 Theme=Dark.

### Icons
- `Icon/close` · `back` · `more` · `search` · `history` · `download` · `plus` · `sparkle` · `chevron-right` · `arrow-up` · `heart` · `comment` · `share` · `grid` · `filter` · `album` · `friends` (24 기준)
- **Icon/bestcut** — `Color(V)` Pink | Green | Purple. 베스트컷 심볼(꽃). 꽃잎마다 카테고리 옅은 색 → 기본색 그라데이션, 불투명도 70%. 브랜드 심볼이라 흰색·검정으로 덮어쓰지 않아요.
- **Icon/like** — `Color(V)` Pink | Green | Purple. 좋아요 3D 유리 8각 배지(꽃 배지). 앨범 카테고리 색에 맞춰 고르고, 흰색·검정으로 덮어쓰지 않아요.
- 카테고리와 색: 취미(Figma 값 `덕질`)=Pink, 업무=Green, 친목=Purple. 기타와 사용자가 추가한 카테고리는 Figma variant가 없고, 프로토타입에서 고른 색(기타는 Outline)으로 칠해요.

### Chip
- **속성:** `Theme(V)` Light | Dark · `State(V)` Default | Selected | All | Pressed | Disabled · `Label(T)` ("베스트컷") · `Show Icon(B)` (false) · `Icon(Swap)`
- **모양:** Light 높이 40, 좌우 16 (`lg`), 아이콘–글자 4 (`xs`), 칩 사이 8 (`sm`), `label-md`. Dark(AI 액션 칩) 높이 36, 좌우 12 (`md`).
- **상태:** Light Default=`surface-translucent`, Selected=`primary` + 흰 글자, All=바탕 없이 그리드 아이콘 + 글자, Pressed=바탕 `border`, Disabled=글자 `disabled`. Dark Selected=`neutral` 바탕 + `primary` 글자, Pressed=`white-alpha-40`, Disabled=글자 `white-alpha-40`.
- **규칙:** 한 줄에 선택 칩은 하나. 칩 그룹 사이는 구분선(Vertical). 홈 카테고리 필터는 이 칩이 아닌 별도 규칙(DESIGN.md Components "홈 카테고리 필터")을 따라요.
- **접근성:** 높이 40이라 누르는 영역을 48로 넓히고, 선택 상태는 색 + 채움 모양으로 함께 보여 줘요.

### Button / Primary
- **속성:** `State(V)` Default | Pressed | Disabled | Loading · `Label(T)` ("새 앨범 만들기") · `Show Icon(B)` (true) · `Icon(Swap)` · `Show Badge(B)` (true)
- **모양:** 높이 54, 알약(`rounded.sm`), 좌우 16, `body-md` 흰 글자. 왼쪽 글래스 배지 + 글자, 오른쪽 끝 아이콘.
- **상태:** Pressed=`primary-pressed` · Disabled=`disabled` 바탕 + `neutral` 글자 · Loading=글자·배지·아이콘을 숨기고 점 3개(`neutral`, 간격 `xs`)만 가운데.
- **규칙:** 한 화면에 Primary 버튼은 하나만 둬요. 위험 동작에는 쓰지 않아요(Danger를 써요).

### Button / Bottom
- **속성:** `Type(V)` Primary | Secondary | Icon Only · `State(V)` Default | Pressed | Disabled | Loading · `Label(T)` · `Show Icon(B)` (true) · `Icon(Swap)`
- **모양:** 화면 하단 고정, 높이 56 알약, `shadow-sm`. Primary=주요 동작(검정), Secondary=보조 동작(`surface-raised`), Icon Only=56×56 원형(사진 올리기 +).
- **상태:** Primary·Icon Only Pressed=`primary-pressed`, Disabled=`disabled` 바탕, Loading=점 3개. Secondary Pressed=바탕 `border`, Disabled=글자·아이콘 `disabled` (Loading 없음).
- **규칙:** 문구는 다음에 일어날 일을 동사로, 개수가 있으면 넣어요(VOICE.md: '3명에게 보내기', '카테고리 생성'). 스크롤 내용 끝에는 버튼 높이 + 24 여백을 둬요.

### 구분선 (Divider)
- **속성:** `Direction(V)` Vertical | Horizontal
- 1px, `border`. Vertical=칩 그룹 사이(높이 22)·통계 카드 가운데. Horizontal=목록 구분.

### Hint Card
- `surface-raised`, `rounded.md`, 여백 16, `shadow-sm`. 아이콘 24 + 제목(`body-md`) + 설명(`body-sm`, `secondary`).
- 쓰는 곳: 앨범 상세 사진 목록 끝 '마음에 드는 사진이 없나요?'.

---

## 홈

### Logo
- simpic 워드마크, 홈 헤더 왼쪽 105×43.

### Profile Button
- 44×44, `surface` 바탕 + 흰 테두리 2 + `shadow-sm`, 사진 40. 사진은 인스턴스에서 이미지 채우기로 바꿔요.

### Tab Bar
- **속성:** `Selected(V)` 앨범 | 친구
- 홈 하단 탭. 모양·모션은 DESIGN.md Components "Tab Bar"와 Interaction & Motion "Frosted Glide"를 따라요(Neutral 반투명 알약 + 블러, 선택 탭 Neutral Subtle 알약). → Figma 설명과 다른 점은 아래 표를 보세요.

### Album Card
- **속성:** `Category(V)` 덕질 | 업무 | 친목 · `Title(T)` ("생일카페 투어") · `Meta(T)` ("11.01부터 · 86장") · `More Count(T)` ("+83")
- **모양:** 폭 372, 여백 16, `rounded.md`, 카테고리 옅은 색 바탕. 위: 기울어진 사진 3장(−9°~+9°) + More 카드(옅은 색 → `neutral` 그라데이션, `+83`은 카테고리 기본색 `headline-md`). 아래: 제목(`headline-md`) → 카테고리(`label-md`, 기본색) ' | ' 날짜(`label-md`, `secondary`) + 오른쪽 아래 Avatar Stack. 카드 사이 12 (`md`).
- **규칙:** 장수는 쓰지 않아요(DESIGN.md). 카테고리 라벨 글자는 `pink-text`(취미)·`green-text`(업무)·`purple`(친목)을 써요. 취미 `+83`은 `pink-vivid`. 사용자가 추가한 카테고리는 고른 색으로 바탕·라벨·`+N`을 만들어요(DESIGN.md Colors).

### Avatar Stack
- **속성:** `Style(V)` Pink | Green | Purple · `Count(T)` ("+4")
- 앨범 카드용: 30px 원형, −8 겹침, 흰 테두리 2, 마지막 `+N` 배지는 카테고리 기본색 바탕 + `body-sm` 숫자(취미·업무는 검정, 친목은 흰색 — 대비가 높은 쪽).
- 그룹 행용: 32px, −9 겹침, `surface` 테두리, `+N` 배지는 Green 바탕 + 검정 숫자.

### Group Row
- 그룹 목록 행. 높이 70, `surface` 바탕, `rounded.md`, 좌우 16. 그룹 이름(`body-md`) + 메타(`body-sm`, `secondary`) + 아바타 + 오른쪽 화살표. 행 사이 8 (`sm`).

---

## 친구

### Friend Row
- **속성:** `Initial(T)` ("도") · `Name(T)` ("도윤") · `Sub(T)` ("함께한 공유 앨범 4개") · `Show Sub(B)` (false)
- 친구 탭 목록 한 줄. 카드 없이 흰 바탕에 바로 놓아요. 아바타 44 + 이름(`body-md`) + 보조(`body-sm`) + 더보기. 설정의 친구 목록도 같은 행을 써요.

### Group Row / 친구 탭
- **속성:** `Name(T)` ("대학 동기") · `Meta(T)` ("앨범 8개 · 5명") · `Count(T)` ("+2") · `Show Count(B)` (true)
- 친구 탭 위쪽 '자주 모이는 그룹' 행.

---

## 앨범 상세

### Album Hero
- **속성:** `Category(V)` 덕질 | 업무 | 친목 · `Title(T)` · `Date(T)`
- 카테고리 옅은 색 → `neutral-subtle` 그라데이션 위에 꽃 그래픽 에셋 2장(오른쪽 위 110×192, 왼쪽 80×144, 원본 그대로) + 위에서부터 제목(`headline-lg`, 가운데) → 카테고리(`label-md`, 기본색)·날짜(`label-md`, `secondary`) → 사진 콜라주.
- 장식 오브젝트는 카테고리별 에셋으로 바꾸고 토큰 색으로 칠하지 않아요. 장식은 스크린리더가 건너뛰게 해요.
- Figma에는 취미(덕질)·업무·친목 3개만 있어요. 프로토타입에서는 기타(회색 그래픽)와 사용자가 추가한 카테고리(기본 그래픽을 흰색 위 고른 색 약 12% 파스텔로 다시 칠함)도 그래픽을 보여 줘요.

### 앨범 상단 · 친목
- 앨범 상세 상단 전체(친목 기준): 상태바 + 뒤로·더보기(Translucent 44) + 제목·카테고리 줄 + 대표 사진 콜라주 + Stats Card + 필터 줄. 폭 412.

### 앨범 필터 줄 (템플릿)
- 컴포넌트가 아닌 배치 견본이에요. 검색 버튼(Icon Button 40) + '전체' 칩 + 구분선 + 베스트컷·좋아요·인물별 칩.
- 탭이 넘치면 오른쪽 끝 64를 흐리고, 밀어서 왼쪽이 가려지면 왼쪽 40도 흐려요. 필터 칩을 길게 누르거나 + 버튼을 누르면 '필터 수정' 시트가 올라와요.

### Stats Card
- `surface-translucent`, `rounded.md`, `shadow-sm`, 위아래 16. 왼쪽 함께한 사람(30px 아바타 −8 겹침 + 카테고리 기본색 `+N` 배지) | 가운데 구분선 | 오른쪽 사진 수(`headline-lg`). 라벨은 `body-sm` `secondary`.
- 배지 색은 앨범 카테고리에 맞춰 바꿔요. 라벨 문구는 '함께한 사람 N명'(VOICE.md 용어집).

### Top 3 Stack
- 128×178 카드 3장, 흰 테두리 2.5, `rounded.md`, `shadow-sm`, 양옆 ±8° 기울기, 뒤쪽일수록 흐리게(80%·50%). 사진은 인스턴스에서 바꿔요.
- 섹션 제목은 '반응이 가장 많은 사진'(VOICE.md 6장). 카테고리별 다음 섹션 제목은 VOICE.md를 따라요(취미: '좋아하는 순간이 잘 담긴 사진').

### Photo Thumbnail · 사진 그리드
- Photo Thumbnail: 정사각형, `rounded.md`. 이미지는 인스턴스에서 바꿔요.
- 사진 그리드: 3열, 칸 사이 8 (`sm`), 칸 = Photo Thumbnail, 폭 372 → 칸 (372 − 16) ÷ 3 ≈ 118.7. 줄은 인스턴스를 복제해 늘려요.
- **접근성:** 칸마다 버튼 역할 + 이름 '날짜 · 장소 · 사진, 좋아요 N개'. 선택 모드에서는 '선택됨/선택 안 됨'도 읽어요.

---

## 사진 상세 · 베스트컷 만들기 [다크 예외]

### Comment Chip
- **속성:** `Avatar(V)` Pink | Green | Purple · `Initial(T)` ("하") · `Comment(T)` ("분위기 영화 같다")
- 높이 40, 흰 20% 유리(`white-alpha-20` + 테두리 `white-alpha-20`), 아바타 32(카테고리 옅은 색 + 흰 테두리 2) + `label-md` 흰 글자. 칩 사이 8.

### Action Bar Item
- 사진 상세 하단 액션 바의 버튼. 아이콘 22 + `body-sm` 흰 글자, 간격 4 (`xs`). 바는 흰 20% 유리 알약, 위아래 12 (`md`)·좌우 24 (`xl`), 양 끝 정렬.

### Blurred Background
- 화면 전체에 까는 흐린 사진(레이어 블러 40). 화면 프레임 맨 뒤에 절대 위치로 둬요. 바탕색은 정하지 않아요.

### Photo Canvas
- 베스트컷·사진 상세의 큰 사진 캔버스. `rounded.lg`, 폭 372, 화면에 남는 높이를 채워요.

### Prompt Input
- 베스트컷 입력창. 높이 60 알약, 흰 20% 유리. 안내 글자 `white-alpha-78`(2026-11-16, Figma는 `white-alpha-40`), 입력된 글자는 `dark.white`. 오른쪽 44×44 AI 생성 버튼(Pink → Pink Light 원형 그라데이션).
- **Loading(B, 기본 꺼짐):** 켜면 AI 생성 버튼 위에 점 3개 오버레이. 생성 중 문구는 '지우는 중이에요…' 같은 현재형(VOICE.md "진행 중")으로 바꾸고 `white-alpha-40`으로 둬요.
- **접근성:** 안내 글자도 정보를 주므로 어두운 바탕에서 읽히게 해요(사용성 테스트 7번).
- 얼굴이 없는 사진에는 얼굴 보정 AI 칩을 보여 주지 않아요.

---

## 색 견본

- 프레임 `색 · Success · Danger · 카테고리 팔레트` (1640:3022)
  - 역할 색: `colors/success`(Success · 토글 켜짐 — 지금 화면에서는 쓰지 않는 예비 색), `colors/danger`(위험 동작 글자)
  - 카테고리 팔레트(사용자가 추가하는 카테고리): `palette/pink · purple · green · orange · sky · teal · yellow · coral · lilac · gray`. 값은 DESIGN.md Screens "카테고리 설정"을 따라요.

## Figma에 컴포넌트가 없는 요소

DESIGN.md에 규칙은 있지만 Figma 컴포넌트로는 아직 없는 것들이에요. 프로토타입 코드와 DESIGN.md를 기준으로 만들어요. `[팀 확인]`
- Toggle (50×30, 켜짐 `primary`, 꺼짐 `outline` #8A8A92)
- 홈 칩 줄의 '+ 카테고리' 칩과 '카테고리 설정' 태그 아이콘 버튼 (사용성 테스트 5번)
- 앨범 만들기 진행 표시(1/4 ~ 4/4), 사진 확인 화면의 빠진 사진 이유 표시, '앨범이 만들어졌어요' 표시
- 약관 동의 체크 목록과 조건 안내 글자
- Bottom Sheet, 확인 창(모달), 토스트, 더보기 드롭다운 메뉴
- 선택 바(전체 선택 · N장 선택됨 · 저장 · 지우기 · 닫기)
- 날짜로 이동 휠, 입장 비밀번호 숫자 4칸 입력란, 검색 입력창

## Figma와 DESIGN.md가 다른 곳

Figma 설명이 최종 프로토타입보다 예전 값으로 남아 있는 곳이에요. 코드와 화면은 **DESIGN.md**를 따르고, Figma 설명은 팀이 고쳐요. `[팀 확인]`

| 컴포넌트 | Figma 설명 | DESIGN.md (따를 값) |
|---|---|---|
| Album Card · 사진 그리드 · Photo Canvas | 폭 350 | 폭 372 (콘텐츠 폭) |
| Album Card | 카테고리 라벨·제목·'날짜·장수' | 제목 → 카테고리 ' \| ' 날짜, 장수는 쓰지 않음 |
| Album Card · Album Hero 기본 글자 | '생일카페 투어' | 예시 앨범 이름은 '콜라보 카페' (VOICE.md 6장) |
| Tab Bar | 350×56, `primary`(검정) 알약, 비선택 `disabled` 글자 | 약 256×58 `neutral` 반투명 알약 + 블러, 선택 `neutral-subtle` 알약, 비선택 `secondary` 글자 |
| Header Album | 뒤로 + 선택·더보기 | 뒤로 + 더보기 (헤더에 '선택' 버튼 없음, 더보기 › 사진 선택) |
| Stats Card | '참여자' | '함께한 사람' (VOICE.md 용어집) |
| Avatar Stack Group | `+N` 배지 청록 #2E8C7E | `+N` 배지 Green (DESIGN.md 20색 밖의 값을 쓰지 않음) |
| Icon Button · Chip · 버튼 Focus | iOS VoiceOver 기본 표시 | 기준 기기는 갤럭시(Android) → TalkBack 기본 표시 |
| 카테고리 이름 (Album Hero · Album Card variant) | 덕질 | 취미 (2026-11-16) |
| Album Card 카테고리 라벨 | 카테고리 기본색 | `pink-text`·`green-text` (Purple은 그대로) |
| Avatar Stack `+N` 숫자 | 흰색 | 취미·업무는 검정 (대비) |
| 위험 색 (`colors/danger`) | #E4444C | #D12F38 |
| Prompt Input 안내 글자 | `white-alpha-40` | `white-alpha-78` |
| Button / Bottom 기본 글자 | '사진 전체 다운로드' | 앨범 하단에 이 버튼을 두지 않음. 전체 저장은 더보기 › '전체 사진 저장하기' |
