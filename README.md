# React Product & Board Project

React를 활용하여 제작한 **상품 목록 및 게시판 웹 프로젝트**입니다.
React Router를 이용해 페이지를 구성하고, 페이지별 컴포넌트를 기능 단위로 분리했습니다.

---

## 프로젝트 소개

React의 기본 구조와 라우팅 방식을 학습하기 위해 제작한 프로젝트입니다.

### 주요 학습 내용

- React 컴포넌트 생성 및 분리
- 페이지 컴포넌트와 UI 컴포넌트 구분
- Props를 활용한 데이터 전달
- 배열의 `map()`을 활용한 목록 출력
- React Router를 활용한 페이지 이동
- URL Parameter를 활용한 상세 페이지 구현
- 존재하지 않는 경로의 404 페이지 처리
- 기능별 폴더 구조 구성

---

## 사용 기술

- React
- JavaScript
- Vite
- React Router DOM
- HTML5
- CSS3

---

## 주요 기능

### 메인 페이지

- 메인 비주얼 영역 출력
- 메인 페이지 전용 컴포넌트 구성

### 상품 페이지

- 상품 목록 출력
- 상품 아이템 컴포넌트 분리
- 상품 상세 페이지 이동
- URL Parameter를 이용한 상품 번호 확인

### 게시판 페이지

- 게시글 목록 출력
- 게시글 행 컴포넌트 분리
- 게시글 상세 페이지 이동
- URL Parameter를 이용한 게시글 번호 확인

### 공통 기능

- 페이지별 컴포넌트 구성
- React Router를 이용한 페이지 이동
- 존재하지 않는 주소의 404 페이지 처리

---

## 페이지 경로

| 경로                   | 페이지        | 설명                 |
| ---------------------- | ------------- | -------------------- |
| `/`                    | Home          | 메인 페이지          |
| `/about`               | About         | 소개 페이지          |
| `/products`            | Products      | 상품 목록 페이지     |
| `/products/:productID` | ProductDetail | 상품 상세 페이지     |
| `/board`               | Board         | 게시판 목록 페이지   |
| `/board/:boardID`      | BoardDetail   | 게시글 상세 페이지   |
| `*`                    | NotFound      | 존재하지 않는 페이지 |

---

## 프로젝트 폴더 구조

```text
src
├─ assets
│
├─ components
│  ├─ about
│  │
│  ├─ board
│  │  └─ BoardTr.jsx
│  │
│  ├─ common
│  │
│  ├─ home
│  │  └─ Visual.jsx
│  │
│  └─ product
│     ├─ ProductItem.jsx
│     └─ style.css
│
├─ pages
│  ├─ About.jsx
│  ├─ Board.jsx
│  ├─ BoardDetail.jsx
│  ├─ Home.jsx
│  ├─ NotFound.jsx
│  ├─ ProductDetail.jsx
│  └─ Products.jsx
│
├─ App.jsx
├─ index.css
└─ main.jsx
```

---

## 폴더별 역할

### `assets`

프로젝트에서 사용하는 이미지, 아이콘 등의 정적 파일을 관리합니다.

```text
assets
→ 이미지, 아이콘, 폰트 등
```

### `components`

페이지를 구성하는 작은 UI 단위의 컴포넌트를 관리합니다.

```text
components/about
→ About 페이지에서 사용하는 컴포넌트

components/board
→ 게시판에서 사용하는 컴포넌트

components/common
→ 여러 페이지에서 공통으로 사용하는 컴포넌트

components/home
→ Home 페이지에서 사용하는 컴포넌트

components/product
→ 상품과 관련된 컴포넌트
```

### `pages`

URL 경로와 연결되는 페이지 컴포넌트를 관리합니다.

```text
Home.jsx
→ 메인 페이지

About.jsx
→ 소개 페이지

Products.jsx
→ 상품 목록 페이지

ProductDetail.jsx
→ 상품 상세 페이지

Board.jsx
→ 게시판 목록 페이지

BoardDetail.jsx
→ 게시글 상세 페이지

NotFound.jsx
→ 존재하지 않는 경로의 404 페이지
```

---

---

## 향후 개선 사항

- [ ] 상품 검색 기능 추가
- [ ] 상품 카테고리 필터 추가
- [ ] 상품 정렬 기능 추가
- [ ] 게시글 작성 기능 추가
- [ ] 게시글 수정 기능 추가
- [ ] 게시글 삭제 기능 추가
- [ ] 장바구니 기능 추가
- [ ] 찜 목록 기능 추가
- [ ] 반응형 웹 구현
- [ ] 로딩 화면 추가
- [ ] 에러 처리 기능 추가
- [ ] 프로젝트 배포

---
