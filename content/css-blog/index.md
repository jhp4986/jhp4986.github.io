---
emoji: 💫
title: About CSS
date: '2023-04-19 00:00:00'
author: Jacob
tags: 블로그 github-pages gatsby
categories: 'HTML&CSS'
---

> # CSS ( Cascading Style Sheets )

- HTML 만으로도 웹 을 만들 수 있지만, 화려한 웹 사이트를 만들려면 HTML 과 CSS 는 뗄 수 없는 관계 이다.
  <br/>
  ( CSS 란 HTML 태그에 디자인 을 입혀주는 것이다. 사람이 옷을 입는것 과 같다.)</br>
  HTML 이 헤더, 문단, 테이블 등으로 정보를 조직화 하는 구조를 제공을 한다면, css 는 html 이 아름다워 보일 수 있도록 html에 스타일을 입히는것이다.<br/>

  ***

  ## CSS 적용 하는 법 👇

  CSS 를 작성한 후 HTML 에 적용되도록 반영하는 3가지 방법이 있다.

```html
      1.  인라인 스타일
		-  html 태그 style 이라는 attribute (속성) 에 직접 작성 할 수 있다.
		<h1 style= “ color: red; “ >. 제목  </h1>

		인라인 스타일을 사용을 하면 다음과 같은 장단점이 있다.
		-빠르고 편하다.
		-하지만 적용해야 할 스타일이 너무 많아지면, 코드의 가독성이 떨어진다.
		-html 태그와 style 코드가 혼재 되어 있어 유지 보수에 약하다.

    		*** style 이 너무 길어서 좋지 않은 코드 예시 ****
	  <h1 style= “ color:red; font-size: 30px;background-color: black;font-weight:bold;“ >
      </h1>
```

```html
2. Style 태그 -html 파일 내에 css 를 작성할 수 있는 방법이다. <style></style> 태그 사이에 CSS 문법을
사용해서 스타일을 작성한다. **
<style>
  h2 {
    color: black;
  }
</style>
** -html 파일에 html 코드도 작성하고, css도 작성을 해서 편하고 빠르다. -기능적으로 (html 구조와
디자인 ) 분리 되지 않았기 때문에 유지보수에 좋지않다. -html 을 수정하려면 html 파일을 확인하고,
디자인을 수정하려면 css 파일을 확인하는 것이 좋다.
```

```html
3. CSS 파일에 작성 - HTML 과 분리 하여 CSS 파일에 따로 작성하는것 - 외부로 분리한 css 파일을 html
파일에 적용하기 위해서는 연결해주는 태그를 html 파일에 추가해 주어야 한다. ***
<link href="style.css" rel="stylesheet" type="text/css" />

- <link /> = 사용할 css 파일을 연결해주는 태그 이다. - href = href 속성에 css 파일 경로를 작성한다.
- rel = rel 은 html 파일과 css 파일의 관계를 설명하는 속성이다. css 파일을 연결할 때는 항상 그
값으로 “stylesheet” 를 입력해야 한다. - type= link 태그로 연결되는 파일이 어떤 것인지 알려준다.
여기서 css 파일을 연결하므로 type 값은 “text/css 이다.
```

## CSS 작성법 👇

스타일을 적용할 선택자( selector ) 를 지정하고, 어떤 스타일을 적용할지 작성한다.

```css
  p{
    color: red;
  }

 p = Selector
 color = Property
 red = Prooperty value
 color: red; = Declaration
```

    **TAG NAME**
     <p> 라는 태그의 내용(텍스트) 을 빨간색으로 바꾼 다는 뜻
    세미콜론 <;> 을 기준으로 여러 종류의 속성을 부여할수 있다.
    color 는 property (CSS 속성) 이고,
    Red 는 그 속성 (property)의 값 (value)이다.
    selector (선택자) 도 여러 종류가 올 수 있다.
    태그 이름도 올수 있고, class 값, 그리고
    id 값도 올수 있다.
    EX.)
    p {
    	font-size: 12px;
    }
    HTML 파일 모든  <p></p> 태그의 글씨 크기가
    12 픽셀로 적용된다.

<br/>
    
        **CLASS NAME**
    selector 가 태그였을 때는 단순히 태그 이름만 적어주엇는데
    class 에 스타일을 적용 하고 싶을 때는 selector 에 
    .(dot) 이 필요하다.

    Ex.)
      .container {
          font-weight: bold;
            }

    class name 은 html 내에서 중복으로 사용 가능하다.
    container 라고 class 가 적용된 태그들은
    모두 글씨가 두꺼워 지게 된다.

<br/>

    **ID NAME **
    id 에 디자인을 적용하고 싶을 때는 selector 에 # 이 필요하다

    Ex.)
      
      #wrap {
          border-width : 1px;
            border-color : blue:
            }
            
    id name 은 class name과 는 다르게 html 내에서 중복으로 
    사용 할 수 없다.
    따라서 id 가 적용된 하나의 요소만 스타일이 적용이 된다.
