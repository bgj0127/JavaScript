# DOM

**DOM**은 Document Object Model의 약자이다.(문서 객체 모델) 

문서 객체 이란 html문서의 태그들을 JavaScript가 이용할 수 있는 객체로 만들면 그것을 문서 객체라고 한다. 

모델을 붙인 이유는 *문서 객체를 인지하는 방식* 이라고 해석 할 수 있다. 

---

### DOM의 구조

DOM은 tree 형식의 자료구조를 가지고 있다. 태그 뿐만 아니라 태그 속 텍스트나 속성 등 모두 node에 속한다. 이 중 HTML 태그를 __요소노드(Element Node)__ 라고 하고, 요소 노드 안에 있는 글자를 __Text 노드(Text Node)__라고 부르기도 한다.


![tree](https://github.com/bgj0127/HTML-CSS/blob/master/JavaScript/DOM.png)


---

### 문서객체 생성

웹 브라우저가 HTML 페이지에 적혀 있는 태그를 읽으면 생성된다. 이 과정은 정적으로 문서 객체를 생성한다 할 수 있다. 

만약 HTML 페이지 없던 문서객체를 JavaScript를 이용하여 생성한다면 동적으로 생성하는 것이 된다. 

* **예시**

```javascript
const header = document.createElement('h1');
//document 객체에 접근하여 <h1> 태그를 생성했다.

const textNode = document.createTextNode('This is DOM');
//document 객체에 접근하여 TextNode를 생성하고 'This is DOM'이라는 스트링을 넣어주었다.

header.appendChild(textNode);
//<h1>태그에 자식노드를 추가해주었다.

document.body.appendChild(header);
//document객체를 통해 body 객체에 접근하였다. body태그에 자식으로 <h1>태그를 추가해주었다.
```



