#### :books: 값으로서 함수와 콜백

* 콜백
* 함수의 동작 방법을 값을 전달하는 것을 통해서 완전하게 바꿀 수 있음

```js
var numbers = [20, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1];
var sortfunc = function (a, b) { //콜백 함수 sortfunc 사용
    return a - b;
};
alert(numbers.sort(sortfunc)); //sort 함수 동작 방법 변경
```
