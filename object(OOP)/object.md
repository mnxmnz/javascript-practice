#### :books: object

* API (Object.keys())
* 인자로 값을 받아서 처리함
<pre>
<code>
var arr = ["a", "b", "c"];
console.log('Object.keys(arr)', Object.keys(arr));
</code>
</pre>

* API (Object.prototype.toString())
* 객체를 만들어서 사용함
<pre>
<code>
var o = new Object();
console.log('o.toString()', o.toString());
</code>
</pre>

* hasOwnProperty
* 객체가 상속받은 프로퍼티인지 직접 정의한 프로퍼티인지 구별할 수 있음
<pre>
<code>
for(var name in o) {
    if(o.hasOwnProperty(name)) {
        console.log(name)l
    }
}
</code>
</pre>
