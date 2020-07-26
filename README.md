# JS_studying
> * [JavaScript]
> * Coding Everybody Language JS
> * https://opentutorials.org/course/743
> * 생활 코딩 언어 JS 강의 실습 코드입니다.
> * 아래 README는 강의 내용 중 일부를 문서로 정리한 것입니다.

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
for(var i = 0; i < 5; i++) {
    var name = 'coding everybody'; //지역 변수의 의미를 갖지 않음
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
    alert(numbers.sort());
</code>
</pre>
* sortfunc 함수의 내용을 인자로 받은 후 내부적으로 호출함
* sortfunc 콜백 함수를 이용해서 sort 함수의 동작 방법을 변경함
<pre>
<code>
    var numbers = [20, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1];
    var sortfunc = function (a, b) {
        return a - b;
    };
    alert(numbers.sort(sortfunc));
</code>
</pre>

## 클로저
* 내부 함수에서 외부 함수의 지역 변수에 접근할 수 있음
* inner 함수에서 title 변수에 접근할 수 있음
<pre>
<code>
function outter() {
    var title = 'coding everybody';
    return function () {
        alert(title);
    }
}
inner = outter();
inner();
</code>
</pre>
* 비밀 변수
* 데이터를 안전하게 저장되고 수정되게 할 수 있음
<pre>
<code>
get_title: function() {
    return title;
},
set_title: function(_title) {
    if(typeof _title === 'String') {
        title = _title
    } else {
        alert('제목은 문자열이어야 합니다.');
    }
}
</code>
</pre>

### 복습 항목 
- [x] 함수지향 - 값으로서의 함수와 콜백 (비동기 콜백과 Ajax)
- [x] 함수지향 - 클로저 (클로저의 응용)