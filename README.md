## :computer: JavaScript

* [Coding Everybody Language JS](https://opentutorials.org/course/743)
* [Coding Everybody Web Browser JS](https://opentutorials.org/course/1375)

### :open_file_folder: Language JS

#### :books: 배열

* 배열에 데이터 한 개 추가하기
<pre>
<code>
배열명.push(' ')
</code>
</pre>

* 배열에 데이터 여러 개 추가하기
<pre>
<code>
배열명 = 배열명.concat(' ', ' ', ' ');
</code>
</pre>

* 배열의 시작점에 데이터 추가하기
<pre>
<code>
배열명.unshift(' ');
</code>
</pre>

* 배열의 중간에 데이터 추가하기
<pre>
<code>
배열명.splice(배열에 추가할 위치를 가리키는 index, 제거될 원소들의 수, ' ', ' ', ' ');
</code>
</pre>

* 배열의 첫 번째 데이터 제거하기
<pre>
<code>
배열명.shift();
</code>
</pre>

* 배열의 마지막 데이터 제거하기
<pre>
<code>
배열명.pop();
</code>
</pre>

* 배열 데이터 오름차순 정렬하기
<pre>
<code>
배열명.sort();
</code>
</pre>

* 배열 데이터 내림차순 정렬하기
<pre>
<code>
배열명.reverse();
</code>
</pre>

#### :books: 유효범위

* 지역 변수를 선언할 수 있는 범위는 함수로 제한되어 있음
* for문이나 if문 내에서 선언된 변수는 지역 변수의 의미를 갖지 않음
<pre>
<code>
for(i = 0; i < 5; i++) {
    var name = 'JS'; //지역 변수의 의미를 갖지 않음
}
</code>
</pre>

* 정적 유효범위
* 함수가 사용된 시점이 아닌, 정의된 시점에서 변수 사용
<pre>
<code>
var i = 5;

function a() {
    var i = 10;
    b();
}

function b() {
    document.write(i);
}

a(); //5 출력
</code>
</pre>

#### :books: 함수

* 메소드
* 객체의 속성 값으로 담겨진 함수
<pre>
<code>
a = {
    b:function(){}
}
</code>
</pre>

#### :books: 값으로서 함수와 콜백

* 콜백
* 함수의 동작 방법을 값을 전달하는 것을 통해서 완전하게 바꿀 수 있음
<pre>
<code>
var numbers = [20, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1];
var sortfunc = function (a, b) { //콜백 함수 sortfunc 사용
    return a - b;
};
alert(numbers.sort(sortfunc)); //sort 함수 동작 방법 변경
</code>
</pre>

#### :books: 클로저

* 내부 함수에서 외부 함수의 지역 변수에 접근할 수 있음
* inner 함수에서 title 변수에 접근할 수 있음
<pre>
<code>
function outter() {
    var title = 'JS';
    return function () {
        alert(title);
    }
}
inner = outter();
inner(); //JS 출력
</code>
</pre>

#### :books: arguments

* 인자의 개수를 알 수 있음
<pre>
<code>
arguments.length
</code>
</pre>

* 인자의 특정 자릿수의 값을 알 수 있음
<pre>
<code>
arguments[i]
</code>
</pre>

#### :books: 생성자

* 객체에 대한 초기화(init)
<pre>
<code>
function Person(name) {
    this.name = name;
    this.introduce = function () {
        return 'My name is ' + this.name;
    }
}
</code>
</pre>

#### :books: this

* 메소드와 this
* 메소드가 소속되어 있는 객체를 가리킨다
<pre>
<code>
var o = {
    func : function () {
        if(o === this) {
            document.write("o === this");
        }
    }
}
</code>
</pre>

* 생성자와 this
* 생성자가 만든 객체를 기리킨다
<pre>
<code>
var o2 = new Func();
if (funcThis === o2) {
    document.write('o2 <br />');
}
</code>
</pre>

#### :books: 상속

* 객체를 생성자의 프로토타입에 할당해서 특정 객체를 상속받음
<pre>
<code>
function Person(name) {
    this.name = name;
}

Person.prototype.name = null;
</code>
</pre>

* prototype
* 객체의 원형(메소드, 프로퍼티)이 저장되어 있음
<pre>
<code>
function Ultra() {}
Ultra.prototype.ultraProp = true;

function Super() {}
Super.prototype = new Ultra();
</code>
</pre>

### :open_file_folder: Web Browser JS

##### :pencil: 복습 (Language JS)

- [x] [함수지향 - 값으로서의 함수와 콜백 (비동기 콜백과 Ajax)](https://www.youtube.com/watch?v=NDFjwybbong)
- [x] [함수지향 - 클로저 (클로저의 응용)](https://www.youtube.com/watch?v=9A0pMrS6Bh0)
- [x] [함수지향 - 함수의 호출 (apply 사용)](https://www.youtube.com/watch?v=Ubs30Xxe-Ps)
- [x] [객체지향 - this (생성자와 this)](https://www.youtube.com/watch?v=TdkYLonYuDw)
- [x] [객체지향 - this (객체로서 함수)](https://www.youtube.com/watch?v=6I421TLN9vg)
- [x] [객체지향 - this (apply와 this)](https://www.youtube.com/watch?v=j0TPsYspzbI)
- [x] [객체지향 - 상속 (상속의 사용법)](https://www.youtube.com/watch?v=mM-4t2J0lYM)

##### :pencil: 복습 (Web Browser JS)
