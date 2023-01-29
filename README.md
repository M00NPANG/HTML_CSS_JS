# Do it! HTML+CSS+자바스크립트 웹 표준의 정석

## HTML 구조 파악하기

+ < !DOCTYPE html> : 현재 문서가 HTML 5 언어로 작성한 웹 문서
  + HTML에서는 영어 대소 문자를 구별하지 않아도 되지만 문서 유형 강조시에 대문자 사용
```
<!DOCTYPE html>
```
+ < html> ~ < /html> : 웹 문서의 시작과 끝을 나타내는 태그
  + < html > : 웹 문서의 시작
  + < /html > : 웹 문서 종료. 태그 뒤 아무 내용도 없어야 함.
  + lang="ko" : 검색 사이트에서 한국어로 제한해 검색할 때 필요( ko = korean )
```
<html lang="ko">
  // 웹 문서 소스 작성
</html> 
```
+ < head > ~ < /head > : 웹 브라우저가 웹 무서를 해석하는 데 필요한 정보를 입력하는 부분
  + 헤드 영역의 내용은 대부분 웹 브라우저 화면에 보이지 않음. 
    + < meta >태그 : 웹 브라우저에는 보이지 않지만 웹 문서와 관련된 정보를 지정할 떄 사용(화면에 글자를 표시할 때 어떤 인코딩을 사용할지 지정하는 것)
      + 웹 서버는 영어가 기본
      ```
      <meta charset="UTF-8"> //한글 사용을 위한 UTF-8 문자 세트 알림
      <meta name="keywords" content="html의 구조"> // 웹 문서의 키워드
      <meta name="description" content="html의 구조를 알아봅시다"> //웹 문서의 설명
      <meta name="author content="MoonPang"> // 웹 문서의 소유자나 제작자 
      ```
                     

+ < body > ~ < /body > : 실제로 웹 브라우저 화면에 나타나는 내용 