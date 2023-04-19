---
emoji: 💫
title: HTML 파일 필수 기본 구성
date: '2023-04-19 00:00:00'
author: Jacob
tags: 블로그 github-pages gatsby
categories: 'HTML&CSS'
---

> ## HTML 파일을 생성하고 페이지를 만들때 꼭 들어가야 하는 기본 구성이다.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title></title>
  </head>
  <body></body>
</html>
```

</br>

    <!doctype html>

⬆️ HTML5 문서임을 브라우저에 알리는 지시어 이다. 반드시 첫번째 줄에 나와야 하고 이것은 HTML 태그가 아니며 대문자 소문자로 구분없이
기입 해도 된다.

```html
<html></html>
```

⬆️ HTML 문서의 전체 범위를 지정하고 Web Browser 가 해석해야 할 HTML 파일의 전체 영역이며 시작과 끝 지점을 알려 주는 역할을 한다.

```html
<head></head>
```

⬆️ head 태그로 둘러싼 부분은 파일의 제목, 본문을 설명하는 메타 태그들, 자바스크립트 코드와 CSS 스타일 시트 등을 포함하며 문서의 본문은 포함되지 않는다.

```html
<title></title>
```

⬆️ HTML 페이지의 타이틀은 페이지의 제목으로, 브라우저의 타이틀 바에 출력된다. 타이틀은 title 태그를 이용하며 head 태그 내에서만 작성된다.

```html
<meta charset="UTF-8" />
```

⬆️ Web Page 저작자, 문자 인코딩 방식, 파일 내용 등 다양한 메타 데이터를 표현하기 위해 사용된다. 이 태그는 name 과 content 속성을 쌍으로 구성한다. 인코딩 방식을 지정할때는 charset 속성을 사용한다.

```html
<body></body>
```

⬆️ Web Browser 가 해석해야 할 HTML 문서의 구조 범위를 지정한다.
</br>
구조란 사용자가 화면을 통해 볼 수 있는 내용 (content) 의 형태나 레이아웃 등을 의미한다.
</br>
[ logo, header, footer, navigation, menu, button, input, popup 등 보이는 모든 것들이 구조에 해당함 ]
</br>
구조는 body 의 범위 안에서만 생성하도록 한다.
자바스크립트 코드를 포함할 수 있고 head 와 body 태그 사이에는 아무것도 들어갈 수 없다.
