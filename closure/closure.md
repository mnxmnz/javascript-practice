#### :books: closure

* 내부 함수에서 외부 함수의 지역 변수에 접근할 수 있음
* inner 함수에서 title 변수에 접근할 수 있음

```js
function outter() {
    var title = 'JS';
    return function () {
        alert(title);
    }
}
inner = outter();
inner(); //JS 출력
```
