# Organizing Data

데이터 정렬엔 2가지 방법이 있다. 바로 Array와 Object가 있다.

### Array

데이터를 리스트같이 저장한다. 

```javascript
const food = ['egg','ham','bread','chicken']
출력결과: egg ham bread chicken

food[2]
출력결과: bread 

food[100]
출력결과: undefined
```



---

### Object

이름에 value를 넣을 수 있다.

```javascript
const myInfo = {
    name:"Giljun",
    age:18,
    gender:"Male",
    address:"Daejeon"
}
출력결과: {name:'Giljun', age:18, gender:'Male', address:'Daejeon'}

myInfo.name
출력결과: Giljun
```

---

Array 속에 Object를 만들 수 있다. 반대로도 가능하다.

```javascript
myInfo {
    favMovies: ["asdf", "sdfe", "wiew"],
    favFood: [
        {
        	name: "Cheese",
            fatty: false
        },
        {
            name: "Kimchi",
            fatty: true
        }
    ]
}
출력결과: favMovies: ['asdf', 'sdfe', 'wiew'],
    	 favFood: [{name: "Cheese", fatty: false },
				   {name: "Kimchi", fatty: true }]

console.log(myInfo.favFood[0].name)
출력결과: Cheese
```

---

상황에 맞는 정렬방법을 사용해야 한다.