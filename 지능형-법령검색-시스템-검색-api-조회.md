# 법령정보지식베이스 지능형 법령검색 시스템 검색 API

- 요청 URL : https://www.law.go.kr/DRF/lawSearch.do?target=aiSearch

### 법령정보지식베이스 지능형 법령검색 시스템 검색 API

요청 변수 (request parameter)

| 요청변수 | 값 | 설명 |
|---|---|---|
| OC | string(필수) | 신청한 API인증값 |
| target | string(필수) | 서비스 대상<br>(지능형 법령검색 시스템 검색 API : aiSearch) |
| type | char(필수) | 출력 형태 : XML/JSON |
| search | int | 검색범위 법령분류<br>(0:법령조문, 1:법령 별표·서식, 2:행정규칙 조문, 3:행정규칙 별표·서식) |
| query | string | 법령명에서 검색을 원하는 질의<br>(정확한 검색을 위한 문자열 검색 query="뺑소니") |
| display | int | 검색된 결과 개수 (default=20) |
| page | int | 검색 결과 페이지 (default=1) |

샘플 URL

1. 법령정보지식베이스 지능형 법령검색 시스템 검색 API XML 조회

[https://www.law.go.kr/DRF/lawSearch.do?OC=test&target=aiSearch&type=XML&search=0&query=뺑소니](https://www.law.go.kr/DRF/lawSearch.do?OC=test&target=aiSearch&type=XML&search=0&query=뺑소니)

2. 법령정보지식베이스 지능형 법령검색 시스템 검색 API JSON 조회

[https://www.law.go.kr/DRF/lawSearch.do?OC=test&target=aiSearch&type=JSON&search=0&query=뺑소니](https://www.law.go.kr/DRF/lawSearch.do?OC=test&target=aiSearch&type=JSON&search=0&query=뺑소니)

출력 결과 필드(response field)

| 필드 | 값 | 설명 |
|---|---|---|
| target | string | 검색서비스 대상 |
| 키워드 | string | 검색 단어 |
| 검색결과개수 | int | 검색 건수 |
| 법령조문ID | int | 법령조문 ID |
| 법령ID | string | 법령ID |
| 법령일련번호 | string | 법령일련번호 |
| 법령명 | string | 법령명 |
| 시행일자 | string | 법령 시행일자 |
| 공포일자 | string | 법령 공포일자 |
| 공포번호 | string | 법령 공포번호 |
| 소관부처코드 | string | 소관부처코드 |
| 소관부처명 | string | 소관부처명 |
| 법령종류명 | string | 법령종류명 |
| 제개정구분명 | string | 법령 제개정구분명 |
| 법령편장절관코드 | string | 법령편장절관코드 |
| 조문일련번호 | string | 법령 조문일련번호 |
| 조문번호 | string | 법령 조문번호 |
| 조문가지번호 | string | 법령 조문가지번호 |
| 조문제목 | string | 법령 조문제목 |
| 조문내용 | string | 법령 조문내용 |
| 법령별표서식<br>ID | int | 법령별표서식 ID |
| 별표서식<br>일련번호 | string | 법령 별표서식일련번호 |
| 별표서식번호 | string | 법령 별표서식번호 |
| 별표서식<br>가지번호 | string | 법령 별표서식가지번호 |
| 별표서식제목 | string | 법령 별표서식제목 |
| 별표서식<br>구분코드 | string | 법령 별표서식구분코드 |
| 별표서식<br>구분명 | string | 법령 별표서식구분명 |
| 행정규칙조문<br>ID | int | 행정규칙조문 ID |
| 행정규칙<br>일련번호 | string | 행정규칙일련번호 |
| 행정규칙ID | string | 행정규칙ID |
| 행정규칙명 | string | 행정규칙명 |
| 발령일자 | string | 발령일자 |
| 발령번호 | string | 발령번호 |
| 시행일자 | string | 시행일자 |
| 발령기관명 | string | 발령기관명 |
| 행정규칙<br>종류명 | string | 행정규칙종류명 |
| 제개정구분명 | string | 행정규칙 제개정구분명 |
| 조문일련번호 | string | 행정규칙 조문일련번호 |
| 조문번호 | string | 행정규칙 조문번호 |
| 조문가지번호 | string | 행정규칙 조문가지번호 |
| 조문제목 | string | 행정규칙 조문제목 |
| 조문내용 | string | 행정규칙 조문내용 |
| 행정규칙<br>별표서식ID | int | 행정규칙별표서식 ID |
| 별표서식<br>일련번호 | string | 행정규칙 별표서식일련번호 |
| 별표서식번호 | string | 행정규칙 별표서식번호 |
| 별표서식<br>가지번호 | string | 행정규칙 별표서식가지번호 |
| 별표서식제목 | string | 행정규칙 별표서식제목 |
| 별표서식<br>구분코드 | string | 행정규칙 별표서식구분코드 |
| 별표서식<br>구분명 | string | 행정규칙 별표서식구분명 |
