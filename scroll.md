### window.scroll or window.scrollTo
```document.querySelector("#up").scrollIntoView({ behavior: "smooth" });```     or       
```window.scroll({ top: 0, left: 0, behavior: 'smooth' });```

scroll()메소드를 이용하여 이벤트 발생시(버튼 클릭 등) 특정 위치로 이동이 가능하게 된다.   


```element.scrollBy({ top: 100, left: 0, behavior: 'smooth' });```   
이렇게 정한 만큼만 이동도 가능하다.
