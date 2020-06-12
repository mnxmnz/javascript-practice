# JS_studying
* [JavaScript]
* Coding Everybody Language JS
* https://opentutorials.org/course/743
* 생활 코딩 언어 JS 강의 실습 코드입니다.
* 아래 README는 강의 내용 중 일부를 문서로 정리한 것입니다.

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
배열명.splice(배열에 추가할 특정 배열의 위치를 가리키는 index, index에서부터 제거될 원소들의 수, ' ', ' ', ' ');
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