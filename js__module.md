# ES6 modules

es6 의 모듈을 사용하기 위해서는,

1.  어떤 파일이 모듈이라는 것을 정의하고 (export)
2.  정의한 파일을 쓸 수 있도록 해야 한다. (import)

## 모듈 정의하기

모듈은 하나의 object 이다. 모듈을 export 하기 위해서는 module.exports 가 모듈 object 를 참조해야한다.

```javascript
let Menu = {};
Menu.specialty = "Roasted Beet Burger with Mint Sauce";

module.exports = Menu;
```

## 모듈 사용하기

정의한 모듈을 사용하기 위해서는 모듈이 정의된 파일을 불러와야 한다. require() 함수를 이용한다.

```javascript
const Menu = require("./menu.js");

function placeOrder() {
  console.log("My order is: " + Menu.specialty);
}

placeOrder();
```
