#### :books: 유효범위

* 지역 변수를 선언할 수 있는 범위는 함수로 제한되어 있음
* for문이나 if문 내에서 선언된 변수는 지역 변수의 의미를 갖지 않음

```js
for(i = 0; i < 5; i++) {
    var name = 'JS'; //지역 변수의 의미를 갖지 않음
}
```

* 정적 유효범위
* 함수가 사용된 시점이 아닌, 정의된 시점에서 변수 사용

```js
var i = 5;

function a() {
    var i = 10;
    b();
}

function b() {
    document.write(i);
}

a(); //5 출력
```
