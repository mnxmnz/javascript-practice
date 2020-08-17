#### :books: 배열

* 함수의 리턴값이 여러 개의 값을 가질 때 사용
<pre>
<code>
var imgs = document.getElementsByTagName('img');
</code>
</pre>

* 배열에 데이터 한 개 추가
<pre>
<code>
배열명.push(' ')
</code>
</pre>

* 배열에 데이터 여러 개 추가
<pre>
<code>
배열명 = 배열명.concat(' ', ' ', ' ');
</code>
</pre>

* 배열의 시작점에 데이터 추가
<pre>
<code>
배열명.unshift(' ');
</code>
</pre>

* 배열의 중간에 데이터 추가
<pre>
<code>
배열명.splice(배열에 추가할 위치를 가리키는 index, 제거될 원소들의 수, ' ', ' ', ' ');
</code>
</pre>

* 배열의 첫 번째 데이터 제거
<pre>
<code>
배열명.shift();
</code>
</pre>

* 배열의 마지막 데이터 제거
<pre>
<code>
배열명.pop();
</code>
</pre>

* 배열 데이터 오름차순 정렬
<pre>
<code>
배열명.sort();
</code>
</pre>

* 배열 데이터 내림차순 정렬
<pre>
<code>
배열명.reverse();
</code>
</pre>
