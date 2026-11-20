<div align="center">

# 🔔 코코벨 (CoCoBell) — 관리자 서비스

**임신 · 육아 기록 서비스 코코벨의 관리자 화면 · API**

</div>

<br>

## 프로젝트

**코코벨**은 임신부터 육아까지 아기의 기록을 가족이 함께 남기는 웹 서비스입니다. 산모수첩 · 하루일기 · 성장차트 · 건강 체크리스트 · 상담 챗봇과 부모 커뮤니티가 있습니다.

이 저장소는 그중 **관리자 서비스**입니다. 서비스 전체 소개, 화면 녹화, 구현 내용은 사용자 API 저장소의 README에 정리했습니다.

👉 **[CS_3_Client_Boot — 코코벨 전체 README](https://github.com/jaann20914-eng/CS_3_Client_Boot)**

| 항목 | 내용 |
| :--- | :--- |
| 기간 | 2025.11.17 ~ 2025.12.11 (약 4주) |
| 인원 | 5명 |

<img src="https://raw.githubusercontent.com/jaann20914-eng/CS_3_Client_Boot/master/docs/readme/architecture.png" alt="코코벨 구성도" width="900">

<br>

## 관리자 기능

| 화면 | API | 내용 |
| :--- | :--- | :--- |
| 대시보드 | `/dash` | 메뉴별 방문 수, 게시글 · 댓글 신고 현황, 회원 연령대 (chart.js) |
| 신고 관리 | `/report` | 신고된 게시글 · 댓글 목록과 상세, 삭제 |
| 회원 관리 | `/user` | 회원 목록, 탈퇴 처리 |
| 로그인 | `/admin/login` | 관리자 로그인 (JWT) |

## 기술 스택

| 분류 | 기술 |
| :--- | :--- |
| **Frontend** | React 19.2, React Router 7, zustand, axios, chart.js 4 + react-chartjs-2, Tiptap |
| **Backend** | Java 21, Spring Boot 3.5, Spring Security + JWT, MyBatis 3, MySQL, Google Cloud Storage |
| **배포** | Firebase Hosting(화면), Cloud Run(API) |

## 팀원

| 이름 | 담당 |
| :-: | :--- |
| [dayun-50](https://github.com/dayun-50) | 관리자 API, 관리자 화면 |
| [tmd0487](https://github.com/tmd0487) | 관리자 대시보드 · 신고 · 회원 화면 |
| [박지원](https://github.com/jaann20914-eng) | 사용자 서비스의 커뮤니티 게시판 · 산모수첩 · 하루일기 (관리자 저장소에는 참여하지 않음) |
| [Fuigang](https://github.com/Fuigang) · [장영서](https://github.com/jangyeongseo) | 사용자 서비스 |

> 이 저장소는 팀 원본 저장소를 fork한 것입니다. 코드는 그대로 두고 README만 정리했습니다.
