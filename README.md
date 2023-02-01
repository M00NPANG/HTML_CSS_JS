# Do it! HTML+CSS+자바스크립트 웹 표준의 정석

## HTML 기본 구조

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
    + < meta >태그 : 웹 브라우저에는 보이지 않지만 웹 문서와 관련된 정보를 지정할 떄 사용
      + 화면에 글자를 표시할 때 어떤 인코딩을 사용할지 지정하는 것!
      + 웹 서버는 영어가 기본
      ```
      <meta charset="UTF-8"> //한글 사용을 위한 UTF-8 문자 세트 알림
      <meta name="keywords" content="html의 구조"> // 웹 문서의 키워드
      <meta name="description" content="html의 구조를 알아봅시다"> //웹 문서의 설명
      <meta name="author content="MoonPang"> // 웹 문서의 소유자나 제작자 
      ```
    + < title >태그 : 헤드 태그 안에서 웹 문서의 제목 입력
      + 웹 브라우저의 제목 표시줄에 표시
      + 해당 페이지의 방문자나 검색 엔진은 제목 표시줄의 제목을 보고 페이지의 전체 내용 추측 가능
      + 웹 사이트의 즐겨찾기 지정시 웹 문서 제목으로 추가됨
      ```
      <title>HTML 기본 문서</title>
      ```                     
+ < body > ~ < /body > : 실제로 웹 브라우저 화면에 나타나는 내용 

## HTML의 기본 구조 자동 생성
+ 첫 번째 줄에 "!"를 입력한 후 tab 또는 enter를 누르면 된다. 다음과 같이 자동 완성된 코드에서 원하는 방식으로 수정하면 된다. 
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  
</body>
</html>
```

## 시맨틱 태그
+ 시맨틱 태그 : 해당 이름만 봐도 의미를 알 수 있는 것
    ex) 텍스트 단락 -> < p >태그, 앵커 -> < a >태그
  + 사용 이유
    1) 웹 브라우저가 HTML의 소스 코드만 봐도 어느 부분이 제목이고 메뉴이고 본문 내용인지 쉽게 알 수 있음
    2) 문서 구조가 정확하게 나뉘어 PC나 모바일의 웹 브라우저와 여러 스마트 기기의 다양한 화면에서 웹 문서를 표현하기 쉬움
    3) 인터넷에서 웹 사이트를 검색할 떄 필요한 내용을 정확히 찾을 수 있음