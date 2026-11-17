---
version: alpha
name: simpic
description: 친구·동료와 함께 사진을 모으고 AI로 베스트컷을 만드는 공유 앨범 앱. 최종 프로토타입(GitHub `index.html`·`existing-user.html`, 2026-11-16 사용성 테스트 반영) 기준. Figma `디자인md 수정용` 페이지 변수는 2026-11-14 기준이라 11-16 변경분(카테고리 글자색·토글·위험 색)은 Figma에 아직 없음.
colors:
  neutral: "#FFFFFF"
  neutral-subtle: "#F5F5F7"
  surface: "#F5F5F7"
  surface-raised: "#FFFFFF"
  surface-translucent: "rgba(255, 255, 255, 0.85)"
  on-surface: "#111114"
  secondary: "#6B6B76"
  border: "#E6E6EB"
  outline: "#8A8A92"
  primary: "#111114"
  primary-pressed: "#6B6B76"
  disabled: "#C8C8CE"
  success: "#30C458"
  danger: "#D12F38"
  pink: "#EE4F9F"
  pink-light: "#FFEBF0"
  pink-opacity: "rgba(238, 79, 159, 0.5)"
  pink-text: "#D6006C"
  pink-vivid: "#FF0080"
  green: "#3A9F0A"
  green-light: "#EDFFD6"
  green-text: "#2A8200"
  purple: "#5B45D4"
  purple-light: "#F0F0FF"
dark:
  white: "#FFFFFF"
  white-alpha-78: "rgba(255, 255, 255, 0.78)"
  white-alpha-60: "rgba(255, 255, 255, 0.6)"
  white-alpha-40: "rgba(255, 255, 255, 0.4)"
  white-alpha-20: "rgba(255, 255, 255, 0.2)"
typography:
  headline-lg:
    fontFamily: SUIT
    fontSize: 28px
    fontWeight: 900
    lineHeight: 36px
    letterSpacing: -0.6px
  headline-md:
    fontFamily: SUIT
    fontSize: 20px
    fontWeight: 800
    lineHeight: 30px
    letterSpacing: -0.5px
  body-md:
    fontFamily: SUIT
    fontSize: 16px
    fontWeight: 700
    lineHeight: 24px
    letterSpacing: -0.3px
  label-md:
    fontFamily: SUIT
    fontSize: 14px
    fontWeight: 700
    lineHeight: 20px
    letterSpacing: 0px
  body-sm:
    fontFamily: SUIT
    fontSize: 12px
    fontWeight: 400
    lineHeight: 16px
    letterSpacing: 0px
rounded:
  sm: 999px
  md: 16px
  lg: 28px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 16px
  page-margin: 20px
  xl: 24px
  2xl: 32px
shadow:
  sm: "0 2px 6px rgba(0, 0, 0, 0.08)"
  md: "0 10px 24px rgba(0, 0, 0, 0.12)"
components:
  page:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.on-surface}"
    padding: "{spacing.page-margin}"
  page-subtle:
    backgroundColor: "{colors.neutral-subtle}"
    textColor: "{colors.on-surface}"
    padding: "{spacing.page-margin}"
  album-title:
    textColor: "{colors.on-surface}"
    typography: "{typography.headline-lg}"
  section-title:
    textColor: "{colors.on-surface}"
    typography: "{typography.headline-md}"
  text-secondary:
    textColor: "{colors.secondary}"
    typography: "{typography.body-sm}"
  divider:
    backgroundColor: "{colors.border}"
    size: 1px
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.neutral}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    height: 54px
    padding: "{spacing.lg}"
  button-primary-pressed:
    backgroundColor: "{colors.primary-pressed}"
    textColor: "{colors.neutral}"
  button-primary-disabled:
    backgroundColor: "{colors.disabled}"
    textColor: "{colors.neutral}"
  button-bottom-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.neutral}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    height: 56px
    shadow: "{shadow.sm}"
  button-bottom-secondary:
    backgroundColor: "{colors.surface-raised}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    height: 56px
    shadow: "{shadow.sm}"
  icon-button:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.sm}"
    size: 44px
  icon-button-translucent:
    backgroundColor: "{colors.surface-translucent}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.sm}"
    size: 44px
    shadow: "{shadow.sm}"
  icon-button-filter:
    backgroundColor: "{colors.surface-translucent}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.sm}"
    size: 40px
  text-button:
    backgroundColor: "{colors.surface-translucent}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    height: 44px
    padding: "{spacing.lg}"
  chip:
    backgroundColor: "{colors.surface-translucent}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    height: 40px
    padding: "{spacing.lg}"
  chip-selected:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.neutral}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    height: 40px
    padding: "{spacing.lg}"
  chip-all:
    backgroundColor: "transparent"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    height: 40px
    padding: "{spacing.lg}"
  group-row:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    height: 70px
    padding: "{spacing.lg}"
  card-hint:
    backgroundColor: "{colors.surface-raised}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: "{spacing.lg}"
    shadow: "{shadow.sm}"
  card-stats:
    backgroundColor: "{colors.surface-translucent}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "{spacing.lg}"
    shadow: "{shadow.sm}"
  album-card-pink:
    backgroundColor: "{colors.pink-light}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "{spacing.lg}"
  album-card-green:
    backgroundColor: "{colors.green-light}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "{spacing.lg}"
  album-card-purple:
    backgroundColor: "{colors.purple-light}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "{spacing.lg}"
  category-label-pink:
    textColor: "{colors.pink-text}"
    typography: "{typography.body-sm}"
  category-label-green:
    textColor: "{colors.green-text}"
    typography: "{typography.body-sm}"
  category-label-purple:
    textColor: "{colors.purple}"
    typography: "{typography.body-sm}"
  count-badge-pink:
    backgroundColor: "{colors.pink}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    size: 30px
  count-badge-green:
    backgroundColor: "{colors.green}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    size: 30px
  count-badge-purple:
    backgroundColor: "{colors.purple}"
    textColor: "{colors.neutral}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    size: 30px
  photo-thumbnail:
    rounded: "{rounded.md}"
  photo-canvas:
    rounded: "{rounded.lg}"
  bottom-sheet:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    padding: "{spacing.page-margin}"
  glass-dark:
    backgroundColor: "{dark.white-alpha-20}"
    borderColor: "{dark.white-alpha-20}"
    textColor: "{dark.white}"
    rounded: "{rounded.sm}"
  chip-dark:
    backgroundColor: "{dark.white-alpha-20}"
    textColor: "{dark.white}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    height: 36px
    padding: "{spacing.md}"
  chip-dark-selected:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    height: 36px
    padding: "{spacing.md}"
  selection-area:
    backgroundColor: "{colors.pink-opacity}"
    borderColor: "{colors.pink-light}"
  tab-bar:
    backgroundColor: "{colors.neutral}"
    borderColor: "{colors.border}"
    rounded: "{rounded.sm}"
    height: 58px
    padding: "{spacing.xs}"
  tab-bar-item-selected:
    backgroundColor: "{colors.neutral-subtle}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
  tab-bar-item:
    textColor: "{colors.secondary}"
    typography: "{typography.body-sm}"
  toggle-on:
    backgroundColor: "{colors.primary}"
  toggle-off:
    backgroundColor: "{colors.outline}"
  photo-cta:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: "0 {spacing.xl}"
  like-badge:
    backgroundColor: "{dark.white-alpha-20}"
    borderColor: "{dark.white-alpha-20}"
    textColor: "{dark.white}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
---

## Overview

친구·동료와 함께 찍은 사진을 한 앨범에 모으고, AI가 고른 베스트컷을 보여 주는 공유 앨범 앱입니다. 화면은 흰색과 아주 옅은 회색 위에 사진이 주인공이 되도록 비워 두고, 앨범 주제(친목·취미·업무·기타)마다 정해진 카테고리 색 한 쌍으로만 분위기를 바꿉니다.

- 기준 기기: 갤럭시(Android), 프레임 412×915, 좌우 여백 20, 콘텐츠 폭 372. 맨 위 삼성 상태바(44), 맨 아래 삼성 3버튼 내비게이션(48)
- 기준: 최종 프로토타입. GitHub 저장소의 `index.html`(처음 사용자)·`existing-user.html`(기존 사용자) 최신 버전(2026-11-16, 사용성 테스트 1~10번 반영)입니다. 이 문서는 이 프로토타입과 같은 내용입니다. 아래 시안과 프로토타입이 다르면 프로토타입을 따릅니다.
- 카테고리 이름: 2026-11-16부터 '덕질'을 '취미'로 바꿨습니다(드러내고 싶지 않은 사람을 배려). 앨범 이름 자동 분류에서는 '덕질'이라고 입력해도 취미로 분류합니다. Figma 레이어·variant 이름에는 아직 '덕질'이 남아 있습니다.
- 참고 시안: 팀이 확정한 `최종화면` 묶음 (2026-11-14)
  - 홈: `[하단바 시안 A · 글래스 + 점 표시]`(앨범 탭), `[Claude 개선안] 친구 탭 · 삼성`(친구 탭 — 이 화면의 iPhone 상태바는 참고하지 않음)
  - 앨범 만들기: `앨범 만들기 1/3 · 기본 정보 / 입력 완료 / 시안`, `2/3 · 앨범 탭`, `3/3 · 사진 모으기`, `AI 기준 직접 설정`, `사진 직접 고르기`, `앨범 완성 · 초대`, `친구 목록에서 초대`
  - 앨범 상세: `앨범 · 상단 (커버)`(친목·취미·업무), `앨범 · 스크롤 상태 (필터 고정)`, `앨범 검색`, `앨범 카테고리 설정`
  - 그룹·프로필: `그룹 상세 · 대학 동기 / 더보기 메뉴 / 스크롤`, `내 프로필`, `친구 프로필 · 지민`
  - 다크 화면: `사진 상세 · 비슷한 사진`·좋아요 상태들(사진 상세), `[토큰 적용] 베스트컷(수정)`·`[design.md] 베컷만들기 - 뒤 인물 지우기`(베스트컷 만들기), `문서 사진 상세`·`문서 사진 · 사진 정보`
  - 밝은 단계 화면: `문서 스캔 · 영역 맞추기`, `문서 스캔 · 보정·저장`
  - 302×653 축소본 화면은 412 기준으로 환산해 읽습니다(×1.37).
- 디자인 키워드: 둥근 알약 버튼, 살짝 기울어진 폴라로이드 사진, 사진 위의 반투명 유리 버튼
- Figma 연결
  - 변수: 컬렉션 `Primitive`(원본 값) → `Semantic`(이 문서와 같은 이름, Light 모드 하나). 화면은 `Semantic`만 쓰고, 다크 예외 화면만 `Primitive`의 흰색 계열을 씁니다.
  - 글자: 텍스트 스타일 5개. 그림자: 효과 스타일 `shadow-sm`·`shadow-md`(값은 `shadow/*` 변수에 묶임).
  - 컴포넌트: 같은 페이지 `Components` 섹션. 목록과 사용법은 [component.md](component.md).
- 다크 모드는 없습니다. 다크 화면은 아래 "예외 — 다크 화면" 규칙을 따릅니다.

## Colors

UI 역할색 14개와 카테고리 색 10개, 모두 24개입니다. 이 밖의 색은 만들지 않습니다. 다크 화면 전용 흰색 계열 5개는 "예외 — 다크 화면"에 따로 둡니다.

**바탕과 면**
- **Neutral (#FFFFFF):** 홈 등 기본 페이지 바탕.
- **Neutral Subtle (#F5F5F7):** 앨범 상세처럼 사진이 많은 페이지 바탕. 값은 Surface와 같지만, 페이지 바탕 역할로 따로 둡니다.
- **Surface (#F5F5F7):** 흰 바탕 위의 카드·행·아이콘 버튼 (그룹 행, 검색 버튼, 프로필 버튼).
- **Surface Raised (#FFFFFF):** 회색 바탕(`neutral-subtle`) 위에 올라오는 흰 카드·버튼 (안내 카드).
- **Surface Translucent (흰색 85%):** 사진이나 그라데이션 위에 뜨는 칩·버튼·통계 카드.

**글자와 선**
- **On-surface (#111114):** 기본 글자와 아이콘. 흰 바탕 대비 18.85:1.
- **Secondary (#6B6B76):** 날짜·장수·캡션 같은 보조 글자. 흰 바탕 5.26:1, `neutral-subtle`·`surface` 4.83:1로 항상 4.5:1 이상.
- **Border (#E6E6EB):** 구분선과 1px 테두리.
- **Outline (#8A8A92):** 꺼진 토글 바탕(흰 바탕 3.43:1, WCAG 1.4.11의 3:1)과 '기타' 카테고리 색. 글자에는 큰 글자에만 씁니다.

**동작**
- **Primary (#111114):** 주요 버튼, 선택된 칩, 사진 올리기 버튼. 흰 글자 18.85:1.
- **Primary Pressed (#6B6B76):** 주요 버튼을 누른 상태. 흰 글자 5.26:1. 값은 Secondary와 같습니다(`color/gray/600`).
- **Disabled (#C8C8CE):** 비활성 버튼 바탕과 비활성 글자.
- **Success (#30C458):** 지금 화면에서는 쓰지 않는 예비 색입니다. 토글이 켜진 상태는 앱 전체(앨범 만들기·친구 초대·앨범 설정·설정·사진 화면 시트)에서 Primary로 통일합니다. 꺼진 토글은 Outline 바탕. 손잡이는 Neutral + `shadow-sm`. (Figma `Semantic` › `colors/success` → `Primitive` › `color/green/400`)
- **Danger (#D12F38):** 되돌릴 수 없는 위험 동작(지우기·끊기·나가기·비우기)의 글자와 아이콘. 설정 화면의 확인 시트·확인 창 위험 동작 버튼('계정 지우기', 'N장 지우기', '비우기')은 Danger 바탕 + 흰 글자로 씁니다(비활성 '비우기'는 Danger 40%). 앨범·그룹·친구 화면의 가운데 확인 창 실행 버튼은 Danger가 아닌 Primary(검정)입니다(아래 '확인 창' 참고). 흰 바탕 5.03:1, 흰 글자 5.03:1. 예전 값 #E4444C(4.02:1)는 접근성 점검에서 더 진하게 바꿨습니다. (Figma `Semantic` › `colors/danger` → `Primitive` › `color/red/500`, Figma 값은 아직 #E4444C)
- **누른 상태(Pressed):** 주요 버튼(검정)은 `primary-pressed`, 그 밖의 밝은 버튼·칩(Surface·Translucent·Surface Raised)은 바탕을 `border`로 바꿉니다. 로딩 상태는 바탕을 그대로 두고 점 3개(불투명도 50%)를 보여 줍니다.

오류 표시가 필요한 화면은 Danger를 씁니다.

**카테고리 색** — 카테고리마다 기본색 + 옅은 색 한 쌍.

| 카테고리 | 기본색 | 옅은 색 | 글자색 |
|---|---|---|---|
| 친목 | Purple #5B45D4 | Purple Light #F0F0FF | Purple (그대로) |
| 취미 | Pink #EE4F9F | Pink Light #FFEBF0 | Pink Text #D6006C |
| 업무 | Green #3A9F0A | Green Light #EDFFD6 | Green Text #2A8200 |
| 기타 | Outline #8A8A92 | Neutral Subtle #F5F5F7 | Secondary #6B6B76 |

- **기본색:** More 카드의 `+83` 글자(취미만 Pink Vivid #FF0080), `+N` 함께한 사람 배지 바탕(취미·업무 배지 숫자는 On-surface 검정, 친목은 흰색), 베스트컷 심볼 그라데이션 끝.
- **글자색:** 카테고리 라벨처럼 카테고리 색으로 쓰는 글자. Pink·Green은 대비가 모자라 같은 색조로 밝기만 낮춘 글자색(Pink Text·Green Text)을 씁니다. 배지 전용 색은 따로 두지 않습니다(예전 `pink-badge`·`green-badge`는 기본색으로 통합).
- **옅은 색:** 앨범 카드 바탕, More 카드 그라데이션 시작, 앨범 상세 상단 그라데이션 시작, 사진 상세 댓글 아바타, 베스트컷 심볼 그라데이션 시작.
- **Pink Opacity (Pink 50%):** 베스트컷의 지울 영역 표시 전용.
- **대비:** Purple은 흰 바탕 6.47:1, Purple Light 위 5.73:1로 글자에 써도 됩니다. Pink(흰 바탕 3.36:1, Pink Light 위 2.94:1)와 Green(흰 바탕 3.42:1, Green Light 위 3.24:1)은 4.5:1에 못 미쳐 **글자에 쓰지 않고**, Pink Text(흰 5.15 · Pink Light 4.51)와 Green Text(흰 4.89 · Green Light 4.63)를 씁니다. 취미 `+83`(headline-md, 큰 글자)은 Pink Vivid(Pink Light 위 3.31:1)로 3:1을 지키고, 업무 `+83`은 Green 그대로 둡니다(3.24:1).
- **사용자가 추가한 카테고리:** 카테고리 설정의 팔레트 10색 중 고른 색으로 같은 한 쌍을 만듭니다. 바탕은 옅게, 라벨 글자는 같은 색조로 진하게(4.5:1), `+N`은 3:1, 배지 숫자는 흰색·검정 중 대비가 높은 쪽. 기본 카테고리의 색을 바꿔도 같은 방식입니다.

## Typography

서체는 **SUIT** 하나만 씁니다. 글자 크기와 줄 높이는 아래 5단계 안에서만 고릅니다. Figma 텍스트 스타일 `headline-lg`·`headline-md`·`body-md`·`label-md`·`body-sm`과 같은 값이며, 각 값은 `typography/*` 변수에 묶여 있습니다.

| 스타일 | 크기 / 줄 높이 | 굵기 | 자간 | 쓰는 곳 |
|---|---|---|---|---|
| headline-lg | 28 / 36 | Heavy (900) | -0.6px | 앨범 상세 제목, 통계 숫자 |
| headline-md | 20 / 30 | ExtraBold (800) | -0.5px | 섹션 제목, 앨범 카드 제목, More 카드 `+83` |
| body-md | 16 / 24 | Bold (700) | -0.3px | 버튼 글자, 그룹 이름, 헤더 제목, 입력창, 탭 바 |
| label-md | 14 / 20 | Bold (700) | 0 | 칩, 앨범 카드 날짜·장수, 메타 정보, 댓글, '저장' |
| body-sm | 12 / 16 | Regular (400) | 0 | 캡션, 더보기 링크, 카테고리 라벨, `+N` 배지, 액션 바 라벨, 헤더 날짜 줄 |

## Layout

- **화면 412×915, 좌우 여백 `page-margin` 20, 콘텐츠 폭 372.** 가로 스크롤 칩 줄도 첫 칩은 20에서 시작합니다.
- **간격은 4의 배수 토큰만 씁니다:** xs 4 · sm 8 · md 12 · lg 16 · xl 24 · 2xl 32 (+ page-margin 20). 이 밖의 여백 값은 만들지 않습니다. 겹침 값(아바타 −8, −9)과 기울기(±4°~±9°)는 장식 배치라 토큰이 아닙니다.
- **세로 리듬**
  - 상태바(44) 바로 아래에 헤더(44)를 붙입니다. 사이 여백 0.
  - 헤더 → 첫 요소 24 (xl)
  - 섹션과 섹션 사이 32 (2xl)
  - 섹션 제목 → 내용 12 (md)
  - 카드와 카드 사이 12 (md), 목록 행 사이 8 (sm)
  - 마지막 요소 → 하단 내비게이션 24 (xl). 하단 내비게이션(48)은 화면 맨 아래에 붙이고 아래 여백은 없습니다.
- **사진 그리드:** 3열, 간격 8 (sm), 칸은 정사각형 ((372 − 16) ÷ 3 ≈ 118.7).
- **화면 구조:** 모든 화면은 세로 오토레이아웃이며 상태바와 하단 내비게이션을 흐름 안에 포함합니다. 겹쳐 놓는 장식(기울어진 사진, 콜라주, 겹친 Top 3 카드, 사진 위 댓글·좋아요)과 다크 화면의 흐린 배경만 자유 배치합니다.
- **누르는 영역:** 보이는 크기와 상관없이 누르는 영역은 48×48 이상입니다(Android 기준, accessibility-guide.md 2.5.8). 44 버튼·40 칩은 보이는 크기는 그대로 두고 누르는 영역만 넓힙니다.
- **상단:** 모든 화면의 상단 버튼은 44×44(누르는 영역 48), 버튼 사이 8. 헤더 제목은 화면 정가운데에 둡니다. 예외로 사진 상세 계열(Header Dark Date)은 제목·날짜를 닫기 버튼 오른쪽에 왼쪽 정렬합니다. 필터 줄의 버튼만 40×40입니다.
- **사진 상세 계열 세로 리듬:** 사진을 크게 보여 주려고 일반 화면보다 좁게 씁니다. 헤더 → 사진 12 (md), 사진 → 하단 줄 16 (lg), 하단 줄 → 하단 내비게이션 16 (lg). 하단 줄은 액션 바(남는 폭)와 오른쪽 CTA 알약(스캔·베스트컷)을 8 (sm) 간격으로 나란히 둡니다.
- **전체 화면 (탭) 상태:** 사진을 탭하면 헤더·하단 줄을 숨기고, `colors/primary` 바탕에 사진을 폭 412로 가운데에 둡니다. 상태바·하단 내비게이션(Dark)만 남깁니다.
- **시스템 UI 예외:** 삼성 상태바와 3버튼 내비게이션은 삼성 UI 키트를 감싼 컴포넌트입니다. 키트 안의 값(안쪽 여백 15·16·18, 간격 10, 시간 글꼴 One UI Sans)은 토큰이 아니며 바꾸지 않습니다. 화면에서는 높이 44·48만 지킵니다.

## Elevation & Depth

그림자는 두 단계만 쓰고, 색은 검정 하나입니다. Figma 효과 스타일로 만들고, 값은 `shadow/sm/*`·`shadow/md/*` 변수에 묶습니다.

- **shadow-sm — `0 2px 6px rgba(0, 0, 0, 0.08)`:** 화면에 살짝 뜬 요소. 프로필 버튼, 앨범 카드 속 사진과 More 카드, 통계 카드, 안내 카드, Top 3 카드, 앨범 상세 원형 대표 사진, 하단 고정 버튼, 사진 위 유리 버튼(밝은 화면).
- **shadow-md — `0 10px 24px rgba(0, 0, 0, 0.12)`:** 더 높이 뜨는 요소. 홈 Tab Bar, 더보기 드롭다운 메뉴, 초대 QR 카드, 내 프로필·친구 프로필의 원형 사진은 `shadow-sm`.
- 배경 블러와 그림자를 함께 쓰는 유리 버튼은 효과 스타일을 쓰면 블러가 사라지므로, 그림자 값만 `shadow/sm/*` 변수에 묶습니다.

그림자 외의 깊이 표현:

- **밝은 화면의 떠 있는 버튼:** 앨범 상세 상단 버튼(뒤로·더보기)과 필터 줄 검색 버튼은 Surface Raised(흰색) + `shadow-sm`이고 배경 블러를 쓰지 않습니다. 앨범 상세를 스크롤해 헤더가 고정되면 두 버튼은 바탕 없이 아이콘만 남습니다. 필터 줄 칩은 블러·그림자 없이 바탕만 씁니다. 배경 블러를 쓰는 밝은 요소는 홈 Tab Bar(Frosted Glide)뿐입니다.
- **앨범 상세 상단 그라데이션:** 카테고리 옅은 색(0%) → `neutral-subtle`(100%).
- **More 카드:** 카테고리 옅은 색 → `neutral` 그라데이션, 흰 테두리 2, `shadow-sm`, −4° 기울기. `+83`은 카테고리 기본색.
- **AI 생성 버튼:** 원형 그라데이션, 가운데 Pink → 바깥 Pink Light.
- **베스트컷 심볼(꽃):** 꽃잎마다 카테고리 옅은 색 → 기본색 그라데이션, 꽃잎 불투명도 70%. 브랜드 심볼이라 흰색·검정으로 덮어쓰지 않습니다. 사진 상세의 '베스트컷' 버튼처럼 '보정하러 가기' 동작에는 꽃 대신 보정(마술봉) 아이콘을 씁니다.

## Shapes

모서리는 세 단계입니다.

- **sm — 999px (완전히 둥글게):** 모든 버튼(하단 고정 버튼 포함), 칩, 입력창, 아바타, `+N` 배지, 상단 아이콘 버튼, 사진 상세 액션 바.
- **md — 16px:** 카드(앨범 카드, 그룹 행, 안내 카드, 통계 카드, More 카드), 사진 썸네일과 그리드 칸, 기울어진 사진.
- **lg — 28px:** 바텀시트 위쪽 모서리, 베스트컷·사진 상세의 큰 사진 캔버스, 초대 QR 카드.

사진은 흰 테두리 2~2.5px를 두르고, 겹쳐 놓을 때는 −9° ~ +9° 사이로 살짝 기울여 폴라로이드처럼 보이게 합니다.

## Components

Figma `Components(수정용)` 섹션에 화면별로 정리돼 있습니다(`공통`·`홈`·`친구`·`앨범 상세`·`베스트컷 만들기`·`사진 상세`). 이름·variant·속성은 [component.md](component.md)를 따릅니다. 아래는 모양 규칙 요약입니다.

- **Status Bar · Navigation Bar:** 삼성 상태바 412×44, 삼성 3버튼 내비게이션 412×48. 둘 다 Light·Dark가 있고, 다크 화면은 Dark를 씁니다.
- **Header:** 412×44, 좌우 20. Home(로고 + 검색·프로필), Album(뒤로 + 더보기 유리 버튼. 스크롤하면 앨범 이름이 뒤로 버튼 옆에 왼쪽 정렬로 나타나고, 두 버튼은 바탕 없는 아이콘만 남음), Dark(닫기 + 가운데 제목 + 보정 기록·'저장'), Dark Date(닫기 + 제목 `body-md`·날짜 `body-sm` 두 줄을 왼쪽 정렬 + 더보기, 사진 상세), Back(뒤로 + 가운데 제목, 내 프로필·문서 스캔 같은 밝은 단계 화면).
- **Button Primary:** 높이 54, Primary 바탕, 흰 `body-md` 글자, 좌우 여백 16, 알약. 왼쪽 글래스 배지 + 글자, 오른쪽 끝 아이콘.
- **Bottom Button (하단 고정):** 높이 56, 알약, `shadow-sm`. 주요 동작은 Primary(검정), 보조 동작은 Surface Raised(흰색). 아이콘 전용 버튼은 56×56 원형 Primary.
- **Icon Button:** 원형. 44(기본)·40(필터 줄). 흰 바탕 위 Surface, 사진·그라데이션 위 Surface Translucent, 다크 화면은 유리(Glass) 또는 바탕 없음(Ghost).
- **Text Button:** 높이 44 알약. 밝은 화면은 Surface Translucent + `body-md`, 다크 화면은 바탕 없이 `label-md` 흰색 40%('저장' 비활성).
- **Chip:** 높이 40, 좌우 여백 16, 아이콘과 글자 사이 4, 칩 사이 8, `label-md`. 기본은 Surface Translucent, 선택은 Primary + 흰 글자. 맨 앞 '전체' 칩은 바탕 없이 그리드 아이콘 + 글자만(아이콘–글자 8). 칩 그룹 사이 구분선은 Border 1px.
- **Album Card:** 폭 372, 안쪽 여백 16 사방, 모서리 md, 카테고리 옅은 색 바탕. 위쪽에 기울어진 사진 3장 + More 카드, 아래쪽에 제목(`headline-md`)과 그 아래 한 줄에 카테고리(`label-md`, 카테고리 글자색) + ' | ' + 날짜(`label-md`, Secondary)를(앨범 상단과 같은 구분선 표기) 4 간격으로 쌓고, 오른쪽 아래에 함께한 사람 아바타. 장수는 쓰지 않습니다. 위쪽 사진 3장 + More 카드는 카드 폭(홈 가로 목록 300, 전체 앨범 보기 372)과 상관없이 좌우 여백이 같도록(카드 가장자리에서 약 10) 고르게 벌려 놓습니다.
- **Avatar Stack:** 30×30 원형 아바타를 −8씩 겹치고 흰 테두리 2px. 마지막은 `+N` 배지(카테고리 기본색 바탕, 숫자 `body-sm`은 흰색·검정 중 대비가 높은 쪽 — 취미·업무 검정, 친목 흰색). 그룹 행 아바타는 32×32, −9 겹침, `surface` 테두리, `+N` 배지는 Green 바탕 + 검정 숫자.
- **Group Row:** 높이 70, Surface 바탕, 모서리 md, 좌우 여백 16. 그룹 이름(`body-md`)과 메타(`body-sm`, Secondary), 아바타, 오른쪽 화살표.
- **Album Hero:** 앨범 상세 상단. 카테고리 그라데이션 배경에 팀이 준 꽃 그래픽 에셋 2장(`앨범 그래픽 {그린|보라|핑크}`는 오른쪽 가장자리 위 110×192, `… 2`는 왼쪽 가장자리 80×144, 원본 그대로·다시 그리지 않음, 업무 그린·친목 보라·취미 핑크. 기타는 같은 그래픽을 Outline 회색으로, 사용자가 추가한 카테고리는 기본 그래픽과 같은 공식(흰색 위 고른 색 약 12%)의 연한 파스텔로 칠합니다. 이때도 베스트컷·좋아요 아이콘은 고른 색을 진하게 유지합니다)을 장식으로 깔고, 그 위에 위에서부터 제목(`headline-lg`, 가운데) → 카테고리(`label-md`, 기본색)·날짜(`label-md`, Secondary) → 사진 콜라주 순서로 둡니다(제목이 사진 위).
- **Stats Card:** Surface Translucent, 모서리 md, `shadow-sm`, 위아래 16. 2칸 + 가운데 Border 구분선. 숫자는 `headline-lg`, 라벨은 `body-sm` Secondary.
- **Top 3 Stack:** 128×178 카드 3장, 흰 테두리 2.5, 모서리 md, `shadow-sm`, 양옆 ±8°. 카드를 누르면 그 사진의 사진 상세가 열립니다.
- **Hint Card:** Surface Raised, 모서리 md, 여백 16, `shadow-sm`, 아이콘 24 + 제목(`body-md`) + 설명(`body-sm`, Secondary).
- **Photo Grid:** 3열, 간격 8, 칸 모서리 md.
- **Bottom Sheet:** Neutral 바탕, 위쪽 모서리 lg, 좌우 여백 20. 하단 버튼은 Bottom Button 규칙을 따릅니다.
- **홈 카테고리 필터:** 흰 바탕 위 칩이라 선택 칩은 Neutral 바탕 + Primary 1px 테두리 + `shadow-sm`(글자 On-surface), 기본 칩은 Neutral-subtle 바탕 + Secondary 글자입니다. 앨범 상세 필터(그라데이션 위)의 반투명 칩과 구분합니다.
- **Tab Bar:** 홈 하단 탭(앨범·친구). 약 256×58 Neutral 알약 + Border 1px 테두리 + `shadow-md`, 안쪽 4 (xs). 화면 가운데, 하단 내비게이션 위 12 (md)에 떠 있습니다. 선택 탭은 Neutral Subtle(옅은 회색) 알약 + On-surface 아이콘·글자, 선택 안 된 탭은 바탕 없이 Secondary 아이콘·글자. 아이콘 22 위 + 글자 `body-sm` 아래.
- **Toggle:** 50×30 알약, 꺼짐 Outline 바탕(3:1), 흰 손잡이 26 + `shadow-sm`. 켜짐은 모든 화면에서 Primary. 스위치 역할 + 이름 + 상태를 함께 읽습니다.
- **다크 화면 요소:** Prompt Input(높이 60 알약, 유리, 오른쪽 44 AI 생성 버튼), AI 액션 칩(높이 36, 좌우 12), Comment Chip(높이 40, 유리, 아바타 32), Action Bar(유리 알약, 아이콘 22 + `body-sm`), Photo Canvas(모서리 lg), 좋아요 배지(유리, 모서리 lg, 사진 오른쪽 아래), CTA 알약(Neutral 바탕, 아이콘 20 + `body-md` On-surface, 높이는 액션 바와 같게).

## Screens

화면별로 정해진 배치와 구성입니다. 컴포넌트 모양은 위 Components, 동작은 아래 Interaction & Motion을 따릅니다.

- **홈 카테고리 칩 선택 테두리:** 선택된 칩의 1px 테두리는 그 카테고리 기본색(친목 Purple, 취미 Pink, 업무 Green, 기타 Outline, 추가한 카테고리는 고른 색). '전체'만 Primary(검정).
- **홈 카테고리 칩 줄:** 칩(높이 40, 좌우 16, `body-md`)이 넘치면 옆으로 스크롤되고 오른쪽 끝은 서서히 흐려집니다. 칩 줄은 위 24 (xl, '새 앨범 만들기'와 칩 사이 간격) · 아래 12 (md) 여백까지 Neutral(흰색) 바탕을 깔고, '새 앨범 만들기' 바로 아래부터 틈 없이 붙여 스크롤해도 위에 고정됩니다. 처음 화면의 첫 앨범 카드는 칩 아래 24에서 시작합니다. 아래로 지나가는 앨범 목록은 이 흰 띠 밑으로 들어가 보이지 않습니다(블러 없음). 홈(앨범·친구 탭) 아래에는 탭 바 위 약 40 지점에서 시작해 탭 바 가운데에서 완전한 흰색이 되는 그라데이션(높이 140)을 하단 내비게이션까지 틈 없이 깝니다. 칩 목록은 카테고리 설정을 따릅니다. 기본 카테고리는 친목·취미·업무·기타 4개이고, 사용자가 추가한 카테고리는 그 뒤에 붙습니다. 칩 줄 맨 끝에는 '+ 카테고리' 칩(새 카테고리 만들기)을 두고, 줄 오른쪽에는 태그 모양 아이콘 버튼(이름 '카테고리 설정')을 둡니다(사용성 테스트 5번).
- **앨범 상세 하단:** 사진 목록 끝은 Hint Card('마음에 드는 사진이 없나요?')로 끝나고(설명용 카드라 누를 수 없음), 사진 올리기 버튼(56 원형, Primary, 플러스)만 오른쪽 아래 20·하단 내비 위 16에 떠 있습니다. 하단에 '사진 전체 다운로드' 버튼은 두지 않고, 전체 저장은 더보기 메뉴의 '전체 사진 저장하기'로 합니다.
- **필터 순서 바꾸기 (필터 수정 시트 · 앨범 설정 필터 수정 · 설정 › 카테고리 수정):** 수정 상태의 필터 칩 왼쪽 손잡이(⠿)를 눌러 끌면 칩이 따라 움직이며 놓은 자리로 순서가 바뀝니다(끄는 동안 칩 불투명도 55%·1.04배). 손잡이에 초점을 두고 ←/→ 키로 한 칸씩 옮길 수도 있습니다. 손잡이를 누르기만 해서는 칩이 빠지지 않고, '전체'는 맨 앞에 고정입니다. '완료'·'저장'을 눌러야 앨범 필터 줄에 반영됩니다.
- **앨범 설정 › 함께한 사람 팀 나누기:** 켜면 앨범 만들기 1/4과 같은 팀 칩(높이 40, Neutral, Border 1px, 입력한 글자 길이에 맞춰 폭이 늘어남, 기본 '청팀'·'홍팀', 최대 12자)과 점선 '+ 그룹 추가'(최대 6개)가 토글 아래에 열립니다. 팀이 3개 이상이면 칩마다 빼기(✕)가 붙습니다. '저장'을 누르면 앨범 필터 줄의 '인물별' 뒤에 '소속별' 필터가 추가되고 그 탭으로 바로 이동하며 "'소속별' 필터를 추가했어요" 토스트가 뜹니다. 끄고 저장하면 '소속별' 필터를 뺍니다. '소속별'은 팀 나누기가 켜진 앨범에서만 '더 넣을 수 있는 필터'에 나옵니다.
- **앨범 소속별 탭:** 위쪽에 팀 칩 줄(팀 이름 + 'N장', `chip` 규칙, 선택은 Primary)을 두고, 고른 팀 사람이 올린 사진을 날짜·시간 묶음으로 보여 줍니다.
- **앨범 베스트컷 탭 · 사진 더보기:** '반응이 가장 많은 사진'과 카테고리별 섹션 2개('좋아하는 순간이 잘 담긴 사진' 등) 제목 오른쪽에 '사진 더보기'(`body-sm` Secondary, 누르는 영역 48)를 둡니다. 누르면 새 화면이 열리고 Back 헤더(가운데 섹션 제목) 아래 '사진 N장'(`label-md` Secondary)과 3열 그리드를 보여 줍니다. '반응이 가장 많은 사진'은 좋아요가 있는 사진을 좋아요 많은 순으로, 칸마다 오른쪽 아래 좋아요 수(3D 꽃 배지 + 숫자)를 붙입니다. 카테고리별 섹션은 섹션에 보이던 사진 다음에 같은 기준의 사진을 더 이어서 보여 줍니다(업무는 '자료가 잘 보이는 사진'에 문서 사진, '현장이 잘 담긴 사진'에 문서 아닌 사진).
- **앨범 인물별 탭:** 사진마다 실제로 나온 사람과 캐릭터로 묶습니다. 위쪽 원형 목록은 사람을 먼저, 캐릭터를 뒤에 두고, 이름 아래 사진 수를 보여 줍니다. 원형 목록(인물별·올린 사람)의 원과 이름 사이는 6이고, 선택된 원만 12로 넓혀 카테고리 색 테두리 바깥선과 이름 사이가 4가 되게 합니다(선택된 원은 1.06배 + 흰 3·카테고리 색 3 테두리). 친구 목록에 있는 사람은 이름(지수, 민지 …), 이름을 모르는 사람은 '사람 1', '사람 2', 사진 속 캐릭터(인형·굿즈·원화 등)는 '캐릭터 1', '캐릭터 2'로 부릅니다. 원 안에는 그 인물이 잘 보이는 사진을 씁니다. 인물이 나온 사진이 없으면 '아직 인물이 나온 사진이 없어요' 빈 화면을 보여 줍니다.
- **비슷한 사진 묶음:** 비슷한 사진이 있는 사진에서만 사진 상세 오른쪽 아래에 묶음(겹친 썸네일 + 장수 배지)을 보여 줍니다. 없으면 묶음을 두지 않고, 저장할 때도 '이 사진만 / 비슷한 사진 모두' 고르기 없이 바로 저장합니다.
- **앨범 장소 탭:** 날짜 줄은 날짜 옆에 장소 이름만 씁니다(예: '8.14 (금) 카페 베이커리'). **올린 사람 탭**의 날짜 줄은 시간만 씁니다(예: '9.26 (토) 오전 10:00'). 시간·장소·장수를 모두 쓰는 건 전체·날짜·인물별 탭입니다. 지도 아래에 장소 칩 줄('전체' + 장소마다 '장소 이름 N장', `chip` 규칙, 선택은 Primary)을 둡니다. 지도 핀(사진이 있는 장소 최대 4개, 라벨 '장소 · 사진 수')이나 칩을 누르면 그 장소에서 찍은 사진만 보여 주고, 고른 핀은 검정 테두리·검정 라벨로 표시합니다. 고른 핀을 다시 누르면 '전체'로 돌아갑니다. 장소 탭이 없는 카테고리(취미)는 그대로 둡니다.
- **앨범 좋아요 탭:** 순위(1~3위 단상)를 두지 않고, 좋아요가 달린 사진을 다른 탭처럼 날짜·시간 묶음(날짜 줄 + 3열 그리드)으로 시간순 나열합니다. 각 사진 오른쪽 아래(가장자리 6)에 카테고리 색 3D 꽃 배지 28.
- **앨범 사진 찾기:** 맨 위 줄(상태바 바로 아래, 앨범 화면 뒤로 버튼과 같은 자리)에 뒤로 버튼(홈 앨범 검색과 같은 아이콘 16, 원 바탕 없음, 누름 영역 44) + 오른쪽에 '‘앨범 이름’에서 사진 찾기' 한 줄(전부 `headline-md`, 뒤로 버튼과 세로 가운데 정렬, 앨범 이름이 길면 이름 부분만 말줄임), 사이 12. 입력 전 화면 섹션 이름은 '이런 걸 찾아볼 수 있어요'(추천 검색어 칩), '필터로 찾아봐요'(필터 칩). 그 아래 12에 검색 입력창(좌우 20, 남는 폭 고정, 높이 48, Surface Raised, 모서리 sm). '닫기' 글자 버튼은 두지 않고, 입력해도 입력창 폭은 바뀌지 않습니다(지우기 버튼 자리를 미리 비워 둠).
- **입장 비밀번호 (모든 화면 공통):** 앨범 만들기 1/4, 앨범 설정, 친구 초대의 '입장 비밀번호' 아래에는 모두 '비밀번호 4자리를 정해 주세요'(`body-sm` Secondary)를 둡니다. 켜면 숫자 4칸 입력란이 바로 아래 열립니다.
- **앨범 친구 초대 (앨범 › 더보기 › 친구 초대):** 헤더 '친구 초대' 아래 제목 '‘앨범 이름’에 친구를 초대해요'(`headline-md`, 가운데, 길면 단어 단위로 두 줄) → 보조 글씨 '앱 없는 친구도 초대할 수 있어요'(`label-md` Secondary, 위 4) → QR 카드(위 24) → 링크 줄(복사) → 보내기 4칸 → 3일 뒤 링크 닫기·입장 비밀번호 카드. 맨 아래 안내문은 두지 않습니다. 앨범 이름과 '지금 함께한 사람 N명' 캡슐은 두지 않습니다. 입장 비밀번호 제목 아래에는 '비밀번호 4자리를 정해 주세요'(`body-sm` Secondary)를 두고, 켜면 앨범 설정과 같은 숫자 4칸 입력란이 바로 아래 열리고, 입력한 번호는 앨범 설정과 같은 값을 씁니다.
- **앨범 설정:** Neutral Subtle 바탕 위 Surface Raised 카드(모서리 md, 안쪽 16, 카드 사이 12). 순서: 커버 → 앨범 이름(Surface 알약 입력 48) → 장소 → 카테고리(한 줄에 4칸 같은 폭, 4개 이하 줄은 왼쪽 정렬, 추가한 카테고리 포함, 선택 Primary) → 필터 수정 → 사진 모으기(호스트만 사진 올리기) → 입장 카드(제목 없이 입장 비밀번호·3일 뒤 링크 닫기 두 줄; 입장 비밀번호 제목 아래에는 '비밀번호 4자리를 정해 주세요'(`body-sm` Secondary)를 두고, 켜면 바로 아래에 앨범 만들기와 같은 숫자 4칸 입력란(칸 52×58, 사이 10, Neutral Subtle, 입력할 칸은 Primary 1.5px 테두리 + Neutral)이 열려 자동으로 입력 상태가 됨) → 함께한 사람 팀 나누기 → '앨범 지우기'(Surface Raised 알약 56, Danger 글자) → 하단 고정 '저장'. 필터 수정 기본 상태는 오른쪽 '편집'(Surface 알약) + Purple Light 칩(Purple 글자). '편집'을 누르면 '완료'(Primary)로 바뀌고 칩에 끌기 표시·빼기(✕)가 붙으며, 구분선 아래 '더 넣을 수 있는 필터'(Surface 점선 칩 + Purple 플러스)가 나옵니다.
- **앨범 만들기 (4단계):** 진행 표시는 실제 단계대로 1/4 ~ 4/4입니다(사용성 테스트 3번).
  - **1/4 기본 정보:** 입력칸 위에 보이는 라벨 '앨범 이름'(`body-md`, 입력칸 안내 글자는 예시 '예: 동창회 가을 소풍', 최대 20자), 모임 칩 위에 라벨 '모임 종류'. 모임 칩은 카테고리 설정의 목록을 그대로 씁니다(기본 친목·업무·취미·기타 + 사용자가 추가한 카테고리). 끝에 점선 '+ 추가' 칩을 한 줄에 둡니다. 카테고리가 4개 이하면 칩이 줄 폭을 나눠 채우고, 5개 이상이면 칩을 글자 폭대로 두고 옆으로 밀어 봅니다(고른 칩이 보이게 스크롤). '+ 추가'로 카테고리 설정에 들어가면 뒤로 가기가 앨범 만들기 1/4로 돌아오고, 거기서 '카테고리 생성'을 누르면 입력하던 내용을 그대로 둔 채 1/4로 돌아와 새 카테고리가 선택됩니다. 날짜를 정하는 휠 아래에는 '지금으로 되돌리기'(글자 링크)와 '완료'(Primary 알약 높이 40, 누르는 영역 48)를 둡니다.
  - **2/4 사진 분류:** 제목 '앨범 안에서 사진을 이렇게 나눠 볼게요', 설명 '앨범 이름을 보고 사진 분류를 추천했어요. 켜 둔 분류가 앨범의 탭이 돼요.' 카드 제목은 '켜 둔 사진 분류'('✦ AI 추천' 표시, '다시 추천' 버튼 없음)이고 켜진 분류 칩에는 × 대신 ✓를 붙입니다. 아래 '더 넣을 수 있는 분류'(사용성 테스트 6번). 이 단계에서만 '필터' 대신 '사진 분류'라고 부르고, 앨범을 만든 뒤 화면(필터 줄·필터 수정·카테고리 설정)은 '필터'를 씁니다.
  - **3/4 사진 모으기:** 제목 '어떤 사진을 모을까요?', 설명 '올리기 전에 한 번 더 확인할 수 있어요.' 선택지 'AI에게 맡기기'(추천) · '직접 고르기' · '앨범 먼저 만들기'(사진 없이 앨범과 초대 링크를 만듦, 버튼이 '앨범 만들기'로 바뀌고 4/4를 건너뜀).
  - **4/4 사진 확인:** 'AI에게 맡기기'와 '직접 고르기'는 항상 이 화면을 거칩니다(사용성 테스트 4번). 제목 '사진 N장을 찾았어요' / 없으면 '아직 모인 사진이 없어요'. AI가 고른 경우 설명은 '선택하신 기준에 따라 골랐어요. 빠진 사진에는 이유가 표시돼요.'이고 빠진 사진에 '…라서 뺐어요' 이유를 붙입니다. 선택한 사진과 빠진 사진의 차이를 크게 보여 줍니다(사용성 테스트 9번). 하단 버튼은 '사진 N장으로 앨범 만들기', 사진이 없으면 '사진은 앨범을 만든 뒤에도 언제든 올릴 수 있어요' 안내와 '사진 없이 앨범 만들기'.
  - **완성(초대):** 제목 위에 '앨범이 만들어졌어요'(체크 아이콘) 표시를 둡니다.
  - '더 넣을 수 있는 분류'는 Surface 바탕 점선 칩 + Purple Light 원 안의 Purple 플러스이며, 마지막에 같은 모양의 '직접 만들기' 칩을 둡니다. 누르면 그 자리가 입력 칩(Neutral, Primary 1px 테두리, 최대 8자, 안내 글자 '분류 이름', 팀 칩처럼 입력한 글자 길이에 맞춰 폭이 늘어남)으로 바뀌고, Enter나 바깥을 누르면 위 '켜 둔 사진 분류'에 들어갑니다(빈 이름은 취소). 1/4 '함께한 사람 팀 나누기'의 팀 칩(높이 40, Neutral, 알약)은 입력한 글자 길이에 맞춰 폭이 늘어나고, 글자 좌우 여백은 16 (lg)으로 같습니다. 1/4 칩은 모두 높이 44, `body-md`, 사이 8로 같은 줄·같은 높이이며, 다섯 칩이 좌우 여백 20 안을 나눠 채웁니다('+ 추가'만 조금 넓게). 3/4 '추천' 배지는 Purple Light 바탕 + Purple `body-sm` 굵게. 완성(QR) 화면은 앨범 친구 초대와 같은 글자 위계로 닫기(원 바탕 없음) → '앨범이 만들어졌어요' → 제목 '‘앨범 이름’에 친구를 초대해요' `headline-md` → 보조 글씨 '앱 없는 친구도 초대할 수 있어요' `label-md` Secondary(위 4) → QR 카드 220(Neutral, 모서리 lg, `shadow-md`) → 링크 줄(Surface 알약 56 + Primary '복사') → 공유 버튼 2×2(Surface, 모서리 md, 높이 52, `body-md`). 입장 비밀번호·질문 안내는 이 화면에 두지 않습니다. '친구 목록'을 누르면 '친구에게 보내기'(전체 선택 Purple, 체크 Primary, 'N명에게 보내기')로 갑니다. 3/4 'AI에게 맡기기'는 카드를 눌러 고르기만 하고, 안의 '기준 직접 설정하기 ›'(Purple)를 눌러야 기준 설정 시트가 올라옵니다.
- **AI 추천 표시:** 앨범 만들기 카테고리 칩 위 'AI 추천' 배지는 Purple 바탕 + 흰 글자. 초대 QR 가운데 사각형도 Purple.
- **날짜로 이동 시트:** 제목 '언제 찍은 사진을 볼까요?' `headline-md`(오른쪽 안내 문구 없음). 아래에 굴려서 고르는 휠 세 칸: 날짜('11월 1일 (일)', 사진이 있는 날짜만), 오전/오후, 시('1시'~'12시'). 휠 글자는 모두 `headline-md`이고 요일 '(일)'만 Secondary, 가운데 선택 띠 Surface(모서리 md), 위아래 항목은 멀어질수록 흐려집니다. 처음에는 지금 보고 있는 사진 묶음의 날짜·시간에 맞춰 열립니다. 버튼 '선택한 시점으로 이동'. 고른 시간에 사진이 없으면 가장 가까운 묶음으로 옮기고 '그 시간엔 사진이 없어서 …로 옮겼어요' 토스트를 띄웁니다. (실제 앱에서 시스템 휠(spinner)을 쓰면 사진 없는 날짜도 보이므로, 직접 만든 휠을 기준으로 합니다.) 날짜로 이동 휠의 오전/오후와 시 칸은 고른 날짜에 실제로 찍은 사진이 있는 값만 보여 줍니다(날짜를 바꾸면 다시 채움). 모든 날짜 휠(날짜로 이동·앨범 만들기)에는 위·아래 버튼을 두지 않습니다. 끄는 동작 대신 위아래에 보이는 값을 눌러서 고를 수 있고, 키보드 위·아래 화살표로도 움직이며, 스크린리더는 지금 값을 읽습니다.
- **카테고리 설정:** 홈 칩 줄 오른쪽의 '카테고리 설정'(태그 아이콘) 버튼, 칩 줄 끝 '+ 카테고리' 칩(바로 새 카테고리), 앨범 만들기의 '+ 추가' 칩에서 엽니다. 목록은 Surface 카드 안 행(색 점 10 + 이름 `body-md` + 그 카테고리를 쓰는 앨범 수 '앨범 N개'(없으면 '아직 앨범 없음') `body-sm` Secondary + 오른쪽 수정(연필)·지우기 아이콘, 화살표 없음. 행이나 연필을 누르면 카테고리 수정 화면), 아래에 점선 '+ 카테고리 추가'. 카테고리를 누르면 세 구역이 같은 제목 스타일('이름'·'색상'·'필터 수정', 모두 `headline-md` On-surface, 위 24·아래 12)로 이어집니다: 이름 입력(입력칸 위에 보이는 라벨 '카테고리 이름', Surface 알약, 입력 글자 On-surface `body-md`) · 색상 고르기(지름 48 원 10개: Pink #EE4F9F, Purple #5B45D4, Green #3A9F0A, Orange #F28C28, Sky #2E9BE6, Teal #14A39A, Yellow #E5B400, Coral #F2665A, Lilac #8A6BD8, Gray #6B6B76, 선택은 Primary 2px 링) · 필터 수정(기본은 Purple Light 칩만, 오른쪽 '수정'(Surface 원형 48×48) → 누르면 '완료'(Primary)로 바뀌며 칩에 끌기 표시·빼기(✕)와 구분선 아래 '더 넣을 수 있는 필터'(점선 + 넣기)가 나오고, '완료'를 누르면 다시 '수정'). 하단 고정 버튼은 기존 카테고리면 '카테고리 지우기'(Surface 알약 56 + 안내 글), 새로 만드는 중이면 '카테고리 생성'(Primary). 새 카테고리는 '카테고리 생성'을 눌러야 목록에 추가됩니다.
- **친구 탭 목록:** '친구 N명'(`headline-md`) 아래 행을 카드 없이 흰 바탕에 바로 놓습니다(아바타 44 + 이름 `body-md` + '함께한 공유 앨범 N개' `body-sm` + 더보기). 행을 누르면 친구 프로필, 더보기(···)를 누르면 설정 친구 목록과 같은 드롭다운(함께한 공유 앨범 보기 | 친구 끊기(Danger))이 뜹니다. 친구 끊기는 확인 창을 거칩니다.
- **그룹 상세 뒤로:** 그룹을 연 화면(친구 탭 '자주 모이는 그룹' 또는 홈)으로 돌아갑니다. 설정의 친구 목록도 같은 목록을 씁니다.
- **내 프로필 · 친구 프로필:** Neutral 바탕, Back 헤더(가운데 제목). 가운데 원형 사진 96(흰 테두리 3 + `shadow-sm`) → 이름 `headline-lg`(내 프로필은 옆에 연필 아이콘) → 이메일 `label-md` Secondary. 아래 섹션은 섹션 이름 `label-md` Secondary + Surface 카드(모서리 md, 행 높이 66 이상, 제목 `body-md` · 보조 `body-sm` Secondary, 오른쪽 화살표). 행 사이 구분선 Border. 친구 프로필은 '함께한 앨범' 목록(썸네일 44, 모서리 md) + '함께 나온 사진' 3열 그리드.
- **설정 (설정 목록·하위 화면·친구 목록):** Neutral Subtle 바탕 위 Surface Raised(흰) 카드, 뒤로 버튼은 Surface Raised 원 44, 행 아이콘은 Surface 타일 34 안의 On-surface 아이콘(AI 항목만 Purple Light 타일 + Purple 아이콘), 토글 켜짐은 Primary. 위험 동작 글자·버튼은 Danger. 친구 목록은 홈 친구 탭과 같은 친구·행(아바타 44 + 이름 `body-md` + 보조 `body-sm` + 더보기)을 흰 카드에 넣고, 더보기(···)는 드롭다운(함께한 공유 앨범 보기 | 친구 끊기(Danger))으로 엽니다. '함께한 공유 앨범 보기'는 친구 프로필로 갑니다. 사진 목록의 선택·지우기 동작은 Interaction & Motion을 따릅니다.

## Interaction & Motion

화면에서 손으로 하는 동작과 움직임의 규칙입니다. 기준은 최종 프로토타입이며, 여기 적힌 시간·크기·순서를 바꾸면 프로토타입도 함께 고칩니다(contract.md "동작 계약").

- **사진 고르기:** 두 가지로 들어갑니다. ① 사진을 길게 누르면(약 0.5초) 선택 상태로 바뀌고 누른 사진이 먼저 선택됩니다. ② 앨범 더보기 메뉴의 '사진 선택'을 누르면 아무것도 고르지 않은 선택 상태로 들어갑니다. 헤더에 '선택' 버튼을 따로 두지는 않습니다. 선택 바는 '전체 선택'(모두 고르면 '선택 해제') · 'N장 선택됨'(없으면 '사진 선택') · 저장(아래 화살표) · 지우기 · 닫기(X) 순서이며, 고른 사진이 없으면 저장·지우기는 흐리게(35%) 둡니다. 저장을 누르면 '사진 N장을 원본 화질로 저장했어요' 토스트 후 선택이 끝납니다.
- **필터 탭 줄 흐림 (앨범 상세):** 탭이 화면 밖까지 이어지면 오른쪽 끝 64를 투명하게 흐려 더 있다는 걸 보여 줍니다. 옆으로 밀어 왼쪽에 가려진 탭이 생기면 왼쪽 40도 흐려지고, 끝까지 밀면 오른쪽 흐림은 사라집니다.
- **사진 찾기 추천 단어:** '이런 걸 찾아볼 수 있어요' 칩과 검색창 예시는 앨범마다 실제 사진에 있는 단어로 둡니다(예: 콜라보 카페 인형·버거·라멘, 속초 여행 바다·산·호수). 찾기 결과는 그 앨범 사진 안에서만 보여 줍니다.
- **자주 묻는 질문 (설정 › 고객센터):** 질문마다 같은 모양의 접고 펼치는 행(높이 58 이상, 질문 `body-md` 굵게, 오른쪽 아래 화살표 18 Secondary). 처음에는 모두 접혀 있고, 누르면 그 아래 답(Surface 바탕, 모서리 sm, `body-sm`)이 열리며 화살표가 위로 돌아갑니다. 여러 개를 동시에 펼칠 수 있고, 다시 누르면 접힙니다.
- **정렬 드롭다운 (그룹 상세 앨범 목록 · 친구 목록):** '앨범' 제목 오른쪽 정렬 버튼('최근 순' + 아래 화살표 14, `label-md` Secondary). 누르면 더보기 메뉴와 같은 모양의 드롭다운이 버튼 아래에 뜨고, 항목은 최근 순 · 오래된 순 · 가나다 순 · 사진 많은 순 4개. 친구 탭의 '친구 N명' 오른쪽에도 같은 모양의 정렬 버튼을 두고 항목은 가나다 순(기본) · 최근에 추가한 순 2개. 지금 정렬 앞에만 체크(22), 나머지는 같은 폭을 비워 글자 줄을 맞춥니다. 고르면 목록이 바로 다시 정렬되고 버튼 글자가 바뀝니다.
- **더보기 메뉴 (모든 화면 공통):** 화면 오른쪽 위 더보기(···)는 어느 화면이든 시트가 아니라 버튼 바로 아래(헤더 아래 8, 오른쪽 20)에 드롭다운으로 뜹니다. 앨범 상세: 전체 사진 저장하기 · 사진 선택 | 앨범 설정 · 친구 초대 · 함께한 사람 팀 나누기 | 앨범에서 나가기(Danger). 그룹 상세: 그룹 이름 바꾸기 | 그룹 나가기(Danger). 친구 프로필: 친구 끊기(Danger). 사진 상세·문서 사진 상세: 앨범 커버로 지정 | 사진 지우기. 공통 모양: 폭 248, Neutral, 모서리 md, `shadow-md`, 안쪽 좌우 16, 항목 높이 56(아이콘 22 + `body-md`, 사이 12), 그룹 사이 Border 구분선. 바깥을 누르면 닫힙니다.
- **앨범 필터 줄의 + 버튼:** 앨범 설정 화면으로 넘어가지 않고, 함께한 사람 시트처럼 아래에서 '필터 수정' 시트가 올라옵니다(제목 `headline-md` + '완료'(Primary), 켜 둔 필터 칩에 끌기·빼기, 구분선 아래 '더 넣을 수 있는 필터'). '완료'를 누르면 바로 필터 줄에 반영됩니다. 필터 칩을 길게 눌러도 같은 시트가 열립니다.
- **좋아요 누름 효과:** 사진 상세에서 좋아요를 누르면 사진 위 여러 곳에 카테고리 색 3D 꽃 배지(34~64)가 좋아요 수만큼(7개 이상이면 7개로 고정) 튀어 오르듯(0.45초, 살짝 넘쳤다 돌아옴) 나타나고, 5초 뒤 1초 동안 서서히 사라집니다.
- **떠 있는 상단 영역:** 앨범 상세를 스크롤할 때 위에 고정되는 헤더·필터 줄에는 배경 블러를 쓰지 않습니다(카테고리 옅은 색 그라데이션만).
- **Tab Bar 모션 (Frosted Glide):** 탭 바 바탕은 반투명 흰색(72%) + 배경 블러 20·채도 180% + Border 테두리의 유리 질감(깜빡임이 없도록 탭 바를 별도 레이어로 고정). 선택 표시(불투명 Neutral Subtle 알약)는 탭을 바꿀 때 0.45초 동안 다음 탭으로 미끄러지며, 이동 중 가로로 살짝 늘어났다(1.14배) 돌아옵니다(살짝 넘쳤다 돌아오는 곡선). 누르는 순간 탭은 0.94배로 눌리고, 선택된 아이콘은 1.08배로 살짝 떠오릅니다.
- **스크롤 끝 여백:** 스크롤 내용이 떠 있는 요소(홈 Tab Bar, 앨범 하단 줄, 하단 고정 버튼) 아래로 지나가는 화면은, 마지막 항목이 가려지지 않도록 그 요소 높이 + 24 (xl)만큼 끝 여백을 둡니다.
- **설정 › 내가 올린 사진:** 월 제목('11월')만 두고 옆에 앨범 이름·장수 줄은 두지 않습니다.
- **설정 사진 선택·지우기:** 선택 상태를 켜고 끄거나 사진을 고를 때 토스트는 띄우지 않습니다(선택 바의 'N장 선택됨'으로 알 수 있음). 설정의 사진 목록(전체 사진·내가 올린 사진)은 사진을 길게 눌러 선택 상태로 들어가고, 칸 오른쪽 위에 앨범과 같은 체크 원(빈 원 → 선택 시 Primary 원 + 흰 체크)을 보여 줍니다. 선택 상태에서는 헤더 자리에 선택 바를 띄웁니다: 왼쪽 '전체 선택'(모두 고르면 '선택 해제', Surface Raised 알약 40 + `label-md`) · 가운데 'N장 선택됨'(`body-md`, 없으면 '사진을 골라 주세요') · 오른쪽 저장(아래 화살표)·지우기(On-surface 휴지통 아이콘, 고른 사진이 없으면 Disabled)와 닫기(X) 원형 버튼 40. 지우기를 누르면 앨범과 같은 확인 창(가운데 모달, Neutral, 모서리 lg, 제목 `body-md` '선택한 N장을 지울까요?' + 설명 `body-sm` '고른 사진만 지워져요. 휴지통에서 30일 안에 되돌릴 수 있어요.' + '계속 보기'(Surface) / 'N장 지우기'(Danger 바탕))이 뜨고, 지운 사진은 목록에서 빠져 휴지통으로 옮겨집니다. 설정의 휴지통 행 숫자와 휴지통 화면(사진 3열 그리드 + 'N장' + '30일이 지나면 완전히 지워져요', '비우기' Danger 활성)이 함께 바뀝니다. 앨범 사진 지우기 확인 창의 지우기 버튼은 앨범의 다른 확인 창과 같이 Primary(검정) 바탕입니다. 설정 화면의 글자도 5단계 스타일만 씁니다(헤더 제목 `body-md`, 시트 제목 `headline-md`, 섹션 이름 `label-md`, 항목 제목 `body-md`, 설명·값·안내문 `body-sm`, 버튼 글자 `label-md`). 사진 위 좋아요 수는 3D 꽃 배지. (내 프로필 화면만 Neutral 바탕 + Surface 카드)
- **사진 올리기 (앨범 오른쪽 아래 +, 빈 앨범의 커버 +):** 아래에서 올라오는 전체 화면. 헤더 닫기(X) + 가운데 '사진 올리기', 아래 '내 휴대폰 사진 N장'(`label-md` Secondary)과 3열 그리드. 사진을 누르면 오른쪽 위 체크 원이 채워지고 카테고리 색 테두리가 생깁니다. 하단 고정 버튼은 고른 게 없으면 '사진을 골라 주세요'(비활성), 고르면 '사진 N장 올리기'(Primary). 올리면 화면이 닫히고 사진이 앨범 마지막 묶음에 들어가며 '사진 N장을 앨범에 올렸어요!' 토스트. 빈 앨범이었으면 처음 올린 사진이 커버가 되고, 홈 앨범 카드의 사진 수와 사진도 함께 바뀝니다.
- **사진 찾기 결과 · 설정 사진 목록:** 결과나 목록의 사진을 누르면 그 사진의 사진 상세가 열립니다(앨범 이름·좋아요 수 그대로).
- **앨범에서 나가기 · 앨범 지우기:** 둘 다 가운데 확인 창(왼쪽 '계속 보기'·'그대로 두기' Surface, 오른쪽 실행 버튼 Primary 검정)으로 묻습니다. 앨범 지우기는 앨범 설정 맨 아래 '앨범 지우기'에서 열고, 제목 '‘앨범 이름’ 앨범을 지울까요?', 설명 '사진 N장과 앨범 기록이 함께한 사람 모두에게서 지워지고 되돌릴 수 없어요.' 실행하면 앨범을 연 화면(홈 또는 그룹 상세)으로 돌아가고 목록에서 빠지며 '‘앨범 이름’ 앨범에서 나갔어요' / '‘앨범 이름’ 앨범을 지웠어요' 토스트.
- **그룹 이름 바꾸기:** 그룹 상세 더보기 › '그룹 이름 바꾸기'. 가운데 모달(제목 `headline-md`, 라벨 '그룹 이름', 입력칸 최대 20자, '그대로 두기' / '저장하기' Primary). 저장하면 그룹 상세 제목과 그룹 목록이 바로 바뀌고 '그룹 이름을 바꿨어요'.
- **그룹 나가기 · 친구 끊기:** 가운데 확인 창으로 묻습니다. 그룹 나가기 '‘그룹 이름’ 그룹에서 나갈까요?' / '그룹 앨범은 그대로 남고, 내 그룹 목록에서만 빠져요', 친구 끊기 '○○님과 친구를 끊을까요?' / '함께 만든 앨범과 사진은 그대로 남아요'. 실행 버튼은 Primary 검정('그룹 나가기', '친구 끊기'), 실행 뒤 이전 화면으로 돌아가고 목록에서 빠집니다.
- **로그아웃 · 계정 지우기:** 설정의 확인 시트에서 실행하면 열린 화면을 모두 닫고 시작 화면(로그인)으로 돌아갑니다. 계정 지우기는 앨범·그룹·친구 목록도 모두 비웁니다.
- **초대 링크로 들어가기 (온보딩 마지막 '초대 링크로 들어가기'):** 1단계 제목 '초대 링크로 들어가기'(`headline-lg`) · '친구에게 받은 초대 링크를 붙여 넣어 주세요' · 라벨 '초대 링크' + 입력칸(Surface 알약 48, 예시 '예: simpic.app/j/K7Q2') · '복사한 링크 붙여 넣기' 칩 · 하단 '앨범 열기'(입력 전 비활성). 링크 형식이 맞지 않으면 입력칸 아래 '초대 링크를 다시 확인해 주세요'(Danger `body-sm`). 2단계는 가운데 정렬로 앨범 커버 원 96 → '‘앨범 이름’에 초대받았어요'(`headline-md`) → '카테고리 · 함께한 사람 N명 · 사진 N장'(`label-md` Secondary) → 라벨 '입장 비밀번호' + '초대한 친구에게 받은 4자리를 입력해 주세요' + 숫자 4칸(칸 52×58, 사이 10, 입력할 칸 Primary 1.5px 테두리) → 하단 '앨범에 들어가기'(4자리 입력 전 비활성). 들어가면 홈 목록 맨 앞에 앨범이 생기고 바로 그 앨범을 열며 '‘앨범 이름’에 들어왔어요!' 토스트.
- **약관 동의 (처음 사용자 온보딩):** 제목 'Simpic 약관에 동의해 주세요'. 필수 항목 3개는 체크가 꺼진 상태로 시작하고, 모두 동의하기 전에는 하단 버튼 '동의하고 계속하기'를 끄고 그 위에 '필수 항목 3개에 동의하면 계속할 수 있어요'(`label-md` Secondary)를 보여 줍니다(사용성 테스트 2번).
- **홈 검색 결과:** 앨범 결과를 누르면 그 앨범으로, 사진 결과를 누르면 사진 보기로 엽니다(사용성 테스트 1번). 결과 이름에는 화면에 보이는 글자를 포함합니다.
- **사진 상세:** 액션 바의 좋아요 버튼은 꽃 아이콘 아래 '좋아요' 글자(`body-sm` 굵게)를 함께 둡니다. 사진 위 댓글 말풍선은 몇 초 뒤 사라집니다(사용성 테스트 8번).
  - 좋아요 버튼의 숫자는 그 사진의 실제 좋아요 수입니다. 0개일 때는 숫자 '0'과 흰색 선만 있는 물결 8각 아이콘(`Icon/like-outline`, 선 굵기 2)을 보여 주고, 누르면 1이 되며 카테고리 색 3D 꽃 배지와 좋아요 효과로 바뀝니다. 문서 사진 상세도 같습니다.
  - 오른쪽 아래 '베스트컷' CTA 알약의 아이콘은 보정(마술봉) 아이콘(`Icon/wand`, 20, On-surface)입니다. 꽃 심볼은 베스트컷 탭·칩 같은 브랜드 표시에만 씁니다.
- **사진 틀 원본 비율 (사진 상세·문서 사진 상세·베스트컷 만들기 전체):** 사진을 잘라내지 않고 원본 비율 그대로 보여 줍니다. 사진 상세·문서 사진 상세는 사진 폭을 항상 화면 좌우 여백 20에 맞추고(폭 372), 높이는 원본 비율대로 정해 원래 사진 자리 안에서 세로 가운데에 놓습니다. 베스트컷 만들기 화면은 원래 사진 자리 안에 비율대로 맞춰 가운데에 놓습니다. 모서리는 `rounded.lg`를 유지합니다. 사진 상세·문서 사진 상세의 좋아요 버튼·비슷한 사진 묶음·댓글 말풍선은 사진 비율과 상관없이 원래 사진 자리의 아래쪽에 고정합니다(가로는 화면 여백 20에 맞춰 헤더 버튼·하단 줄과 같은 선에 둡니다. 댓글 말풍선은 왼쪽 20, 비슷한 사진 묶음과 좋아요는 오른쪽 20. 세로는 원래 사진 자리 아래에서 댓글 말풍선·묶음 16, 좋아요 112, 묶음이 없으면 좋아요 16). 베스트컷 만들기의 지울 영역 표시·결과 배지처럼 사진 속 위치를 가리키는 요소는 맞춘 사진을 기준으로 놓입니다. 사진을 눌러 사진만 보는 상태에서는 화면 전체에 원본 비율로 보여 줍니다.
- **베스트컷 만들기:** 얼굴이 없는 사진에는 얼굴 보정 칩(노출 살리기·눈 뜨게 하기·모두 잘 나온 얼굴로)을 제안하지 않습니다. 결과 화면은 미리보기를 크게 보여 주고, 큰 사진을 좌우로 넘겨 원본과 비교할 수 있으며, 결과 화면에서도 '저장'이 켜져 있습니다(사용성 테스트 7·10번).
- **시트(바텀시트):** 아래에서 올라오고, 뒤의 어두운 막(검정 45%)이나 닫기·완료를 누르면 내려갑니다. 내용을 바꾸는 시트(필터 수정, 날짜로 이동)는 완료·이동을 눌러야 화면에 반영됩니다.
- **남의 사진 지우기:** 고른 사진이 모두 다른 사람이 올린 것이면 확인 창 제목만 '다른 사람이 올린 사진은 지울 수 없어요'(On-surface)로 보여 주고 설명은 달지 않습니다. 버튼은 왼쪽 '그대로 두기'(Surface), 오른쪽 '삭제 요청하기'(Primary)이며, 요청하면 선택이 끝나고 '올린 사람에게 N장 삭제를 요청했어요' 토스트가 뜹니다. 내 사진과 남의 사진이 섞여 있으면 '내가 올린 N장만 지워져요' 창을 씁니다.
- **확인 창(모달):** 되돌리기 어려운 동작(사진 지우기, 앨범 나가기, 휴지통 비우기) 앞에 화면 가운데 모달로 묻습니다. 왼쪽은 그대로 두는 버튼(Surface), 오른쪽은 실행 버튼(Primary 검정 바탕 + 흰 글자, 개수를 넣은 동사: '2장 지우기'). 앨범·그룹·친구 화면의 확인 창(사진 지우기, 앨범 나가기·지우기, 그룹 나가기, 친구 끊기)은 모두 이 규칙을 따르고, 위험하다는 것은 빨간색 대신 제목·설명 글자('되돌릴 수 없어요' 등)로 알립니다. 계정 지우기·로그아웃 같은 설정 동작은 확인 시트로 묻습니다(설정 화면의 위험 버튼은 Danger).
- **토스트:** 동작이 끝났다는 결과만 짧게 화면 아래쪽에 띄웠다가 사라집니다(예: '사진 2장을 휴지통으로 옮겼어요'). 되돌릴 동작이 필요하면 토스트 대신 확인 창을 씁니다.
- **가로 스크롤 줄:** 칩 줄처럼 옆으로 넘치는 줄은 손가락으로 밀거나, 마우스로 끌거나 휠을 돌려 움직입니다. 넘치는 쪽 끝은 서서히 흐려 넘침을 알립니다.
- **스크롤 고정 영역:** 스크롤해도 위에 남는 것 — 홈의 카테고리 칩 줄(흰 띠), 앨범 상세의 헤더·필터 줄(배경 블러 없음), 설정·문서 스캔 단계 화면의 상태바·헤더. 아래에 남는 것 — 홈 Tab Bar(뒤에 흰 그라데이션), 하단 고정 버튼, 사진 올리기 버튼.
- **수정 ↔ 완료 전환:** 편집이 필요한 목록(카테고리 필터, 앨범 설정 필터)은 기본 상태에서 보기만 하고, '수정'(또는 '편집')을 누르면 '완료'로 바뀌며 빼기(✕)·끌기·더 넣을 수 있는 목록이 나타납니다. '완료'를 누르면 같은 화면에서 보기 상태로 돌아갑니다.
- **새로 만들기 vs 기존 고치기:** 새 항목을 만드는 화면(카테고리 추가)은 하단에 '… 생성'(Primary)만 두고, 누르기 전에는 목록에 넣지 않습니다. 기존 항목을 연 화면에만 '… 지우기'(Danger 글자)를 둡니다.

## Do's and Don'ts

- **Do** 새 화면을 만들 때 이 문서, [component.md](component.md), Figma `Semantic` 변수·텍스트 스타일·효과 스타일을 기준으로 삼으세요. 있는 컴포넌트는 인스턴스로 씁니다.
- **Do** `Primitive` 변수는 화면에 직접 연결하지 마세요(다크 예외의 흰색 계열만 허용).
- **Do** 카테고리 색은 한 쌍(기본색 + 옅은 색)으로만 쓰세요. 사용자가 앱에서 추가하는 카테고리는 카테고리 설정의 색 팔레트 10개 중에서 고릅니다(색 점·칩 선택 테두리에 사용). Figma 변수는 `Semantic` › `palette/pink·purple·green·orange·sky·teal·yellow·coral·lilac·gray`이며, 각각 `Primitive`의 500단계(회색은 `color/gray/600`)를 가리킵니다. 견본은 Components(수정용) 섹션 아래 '색 · Success · Danger · 카테고리 팔레트' 프레임에 있습니다.
- **Do** 하단에 고정되는 버튼은 높이 56의 알약 형태로 만드세요.
- **Do** 보조 글자와 밝은 바탕의 입력칸 안내 글자는 Secondary(#6B6B76)를 써서 대비 4.5:1 이상을 지키세요.
- **Do** 누르는 영역은 48×48 이상으로 넓히세요. 아이콘만 있는 버튼에는 이름을 붙이세요.
- **Don't** Pink·Green을 글자색으로 쓰지 마세요. 대비가 4.5:1에 못 미칩니다. 글자에는 Pink Text·Green Text를 씁니다.
- **Don't** 24개 색(+ 다크 예외 흰색 5개, 사용자가 추가하는 카테고리 색 팔레트 10개), 5개 글자 스타일, 7개 간격 값, 3개 모서리 값, 2개 그림자 밖의 값을 새로 만들지 마세요(삼성 상태바·내비게이션 키트 내부 값만 예외). 필요하면 토큰을 먼저 추가합니다([contract.md](contract.md)의 변경 절차).
- **Don't** 버튼을 둥근 사각형으로 만들지 마세요. 버튼은 모두 알약(rounded sm)입니다.
- **Don't** 카테고리 장식 오브젝트(별, 포도, 반짝이 등 3D 이미지)를 토큰 색으로 칠하지 마세요. 카테고리 색에 맞는 이미지 에셋을 따로 씁니다.

## 예외 — 다크 화면 (베스트컷 만들기, 사진 상세)

사진에 집중하는 화면이라 밝은 Semantic 면 토큰 대신 흰색 계열 Primitive 값을 직접 씁니다. 다크 모드는 따로 두지 않습니다.

- 바탕색을 정하지 않습니다. 사진을 화면 전체에 깔고 레이어 블러 40을 줍니다(`Blurred Background`).
- 반투명 유리: 흰색 20% (`color/white-alpha/20`) + 테두리 흰색 20% (1px) + 배경 블러 20. 닫기 버튼, AI 액션 칩, 입력창, 댓글 칩, 좋아요 버튼, 액션 바에 씁니다. 그림자는 쓰지 않습니다. 누른 상태는 바탕을 흰색 40% (`color/white-alpha/40`)로 바꿉니다.
- 글자와 아이콘은 흰색(`color/white`). 비활성 글자('저장')는 흰색 40% (`color/white-alpha/40`). 입력창 안내 글자는 읽혀야 하므로 흰색 78% (`white-alpha-78`)를 씁니다(사용성 테스트 7번: 밝은 바탕 안내 글자는 Secondary, 어두운 바탕은 흰색). 상태바·하단 내비게이션은 Dark를 씁니다. 흰색 60% (`color/white-alpha/60`)는 보조 글자용입니다(사진 상세 헤더의 날짜 줄).
- 선택된 AI 칩만 흰 바탕(`neutral`) + Primary 글자입니다. AI 액션 칩은 높이 36, 좌우 12.
- 지울 영역 표시는 `pink-opacity` 바탕 + `pink-light` 2px 점선.
- 카테고리 색(아바타, 좋아요 3D 꽃 배지, 베스트컷 심볼, AI 생성 버튼)과 간격·모서리·글자 스타일 토큰은 그대로 적용합니다.
