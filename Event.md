# Event



자바스크립트엔 특정 이벤트가 발생했을 시 특정 함수를 실행할 수 있게 해주는 **addEventListener**라는 기능이 있다.

#### 자주 쓰이는 이벤트 목록

* **change** - 변동이 있을 때 발생

* **click** - 클릭시 발생

* **focus**- 포커스를 얻었을 때 발생

* **keydown** - 키를 눌렀을 때 발생

* **keyup** - 키에서 손을 땠을 때 발생

* **load** - 로드가 완료 되었을 때 발생

* **mousedown** - 마우스를 클릭 했을 때 발생

* **mouseout**- 마우스가 특정 객체 밖으로 나갔을 때 발생

* **mouseover** - 마우스가 특정 객체 위로 올려졌을 때 발생

* **mousemove** - 마우스가 움직였을 때 발생

* **mouseup** - 마우스에서 손을 땠을 때 발생

* **select** - option 태그 등에서 선택을 했을 때 발생

  

addEventListener가 특정 이벤트 발생 시 특정 함수를 실행시킨다면, **removeEventListener**는 등록된 이벤트리스너를 *지우는 역할*을 한다.

```javascript
const btn = document.getElementById("myBtn");
btn.addEventListener("click",handleBtn);

function handleBtn(){
    this.style.backgroundColor = "red";
}
```

일반적인 버튼을 클릭하면 버튼의 색이 바뀌는 것을 확인할 수 있다.