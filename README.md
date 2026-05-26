# 홍성규 경기도지사후보 공식 웹사이트
진보당 경기도지사 후보 기호 5번 홍성규의 공식 선거 웹사이트입니다.
홍성규 후보의 출마의 변과 공약을 소개하는 정적 HTML 사이트입니다.

```
├── index.html       # 메인 페이지
├── style.css        # 스타일시트
├── img/             # 이미지 파일
└── schedule/        # 후보 일정 관리 템플릿
```


## 실행 방법
별도의 빌드 과정 없이 `index.html`을 브라우저에서 열거나,
로컬 서버를 실행해서 확인할 수 있습니다.


## 사용 기술

### 라이브러리
| 라이브러리 | 버전 | 용도 |
|---|---|---|
| [Swiper.js](https://swiperjs.com/) | v11 | `index.html` | 이미지 슬라이더 |
| [html2canvas](https://html2canvas.hertzen.com/) | v1.4.1 | `schedule/index.html` | `form`에 입력한 내용을 PNG파일로 출력 
| [Pretendard](https://github.com/orioncactus/pretendard) | v1.3.9 | 웹폰트 |

### 외부 API
| API | 용도 |
|---|---|
| [rss2json](https://rss2json.com/) | 네이버 블로그 RSS를 JSON으로 변환해 보도자료 목록 표시 |

### Vanilla JS
| 기능 | 설명 | 위치 |
|---|---|---|
| IntersectionObserver | 스크롤 위치에 따라 사이드바 메뉴 활성화 | `index.html` |
| Hamburger 메뉴 | 모바일 환경에서 사이드바 토글 | `index.html` |
| Fetch API | 블로그 RSS 피드 비동기 로딩 | `index.html` |
| Drag and Drop API | 일정 항목 순서 변경 | `schedule/index.html` |
| FileReader API | 로컬 이미지 불러오기 및 16:9 자동 크롭 | `schedule/index.html` |
| Canvas API | 크롭된 이미지 처리 | `schedule/index.html` |
| D-day 자동 계산 | 선거일(6/3) 기준 날짜 표시 | `schedule/index.html` |


## 링크
- [라이브 사이트](https://hongseongkyu2026.github.io/hongseongkyu)
- [진보당 공식 홈페이지](http://jinboparty.com)


## 만든 사람
- 정의석, 2026
