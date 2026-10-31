# 법령정보지식베이스 지능형 법령검색 시스템 연관법령 API

- 요청 URL : https://www.law.go.kr/DRF/lawSearch.do?target=aiRltLs

### 법령정보지식베이스 지능형 법령검색 시스템 연관법령 API

요청 변수 (request parameter)

| 요청변수 | 값 | 설명 |
|---|---|---|
| OC | string(필수) | 신청한 API인증값 |
| target | string(필수) | 서비스 대상<br>(지능형 법령검색 시스템 연관법령 API : aiRltLs) |
| type | char(필수) | 출력 형태 : XML/JSON |
| search | int | 검색범위 법령분류(0:법령조문, 1:행정규칙조문) |
| query | string | 법령명에서 검색을 원하는 질의<br>(정확한 검색을 위한 문자열 검색 query="뺑소니") |

샘플 URL

1. 법령정보지식베이스 지능형 법령검색 시스템 연관법령 API XML 조회

[https://www.law.go.kr/DRF/lawSearch.do?OC=test&target=aiRltLs&type=XML&search=0&query=뺑소니](https://www.law.go.kr/DRF/lawSearch.do?OC=test&target=aiRltLs&type=XML&search=0&query=뺑소니)

2. 법령정보지식베이스 지능형 법령검색 시스템 연관법령 API JSON 조회

[https://www.law.go.kr/DRF/lawSearch.do?OC=test&target=aiRltLs&type=JSON&search=0&query=뺑소니](https://www.law.go.kr/DRF/lawSearch.do?OC=test&target=aiRltLs&type=JSON&search=0&query=뺑소니)

출력 결과 필드(response field)

| 필드 | 값 | 설명 |
|---|---|---|
| target | string | 검색서비스 대상 |
| 키워드 | string | 검색 단어 |
| 검색결과개수 | int | 검색 건수 |
| 법령조문ID | int | 법령조문 ID |
| 법령ID | string | 법령ID |
| 법령명 | string | 법령명 |
| 시행일자 | string | 법령 시행일자 |
| 공포일자 | string | 법령 공포일자 |
| 공포번호 | string | 법령 공포번호 |
| 조문번호 | string | 법령 조문번호 |
| 조문가지번호 | string | 법령 조문가지번호 |
| 조문제목 | string | 법령 조문제목 |
| 행정규칙조문<br>ID | int | 행정규칙조문 ID |
| 행정규칙ID | string | 행정규칙ID |
| 행정규칙명 | string | 행정규칙명 |
| 발령일자 | string | 발령일자 |
| 발령번호 | string | 발령번호 |
| 조문번호 | string | 행정규칙 조문번호 |
| 조문가지번호 | string | 행정규칙 조문가지번호 |
| 조문제목 | string | 행정규칙 조문제목 |
