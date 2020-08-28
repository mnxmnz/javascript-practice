#### :books: 상속

* 객체를 생성자의 프로토타입에 할당해서 특정 객체를 상속받음

```js
function Person(name) {
    this.name = name;
}

Person.prototype.name = null;
```

* prototype
* 객체의 원형(메소드, 프로퍼티)이 저장되어 있음

```js
function Ultra() {}
Ultra.prototype.ultraProp = true;

function Super() {}
Super.prototype = new Ultra();
```
