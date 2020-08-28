#### :books: 생성자

* 객체에 대한 초기화(init)

```js
function Person(name) {
    this.name = name;
    this.introduce = function () {
        return 'My name is ' + this.name;
    }
}
```
