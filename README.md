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