# JS_studying

> * [JavaScript]
> * Coding Everybody Language JS
> * Coding Everybody Web Browser JS
> * https://opentutorials.org/course/743
> * https://opentutorials.org/course/1375
> * 생활 코딩 언어 JS & 웹브라우저 JS 강의 실습 코드입니다.
> * 아래 README는 강의 내용 중 일부를 문서로 정리한 것입니다.

# Language JS

## 배열

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

## 유효범위

* 지역 변수를 선언할 수 있는 범위는 함수로 제한되어 있음
* for문이나 if문 내에서 선언된 변수는 지역 변수의 의미를 갖지 않음
<pre>
<code>
for(i = 0; i < 5; i++) {
    var name = 'JS'; //지역 변수의 의미를 갖지 않음
}
</code>
</pre>

* 정적 유효 범위
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

## 함수

* 메소드
* 객체의 속성 값으로 담겨진 함수
<pre>
<code>
a = {
    b:function(){}
}
</code>
</pre>

## 값으로서 함수와 콜백
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

## 클로저
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

## arguments
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

# Web Browser JS

### 복습 (Language JS)
- [x] [함수지향 - 값으로서의 함수와 콜백 (비동기 콜백과 Ajax)](https://www.youtube.com/watch?v=NDFjwybbong)
- [x] [함수지향 - 클로저 (클로저의 응용)](https://www.youtube.com/watch?v=9A0pMrS6Bh0)

### 복습 (Web Browser JS)