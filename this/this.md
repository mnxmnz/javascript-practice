#### :books: this

* 메소드와 this
* 메소드가 소속되어 있는 객체를 가리킴
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
* 생성자가 만든 객체를 가리킴
<pre>
<code>
var o2 = new Func();
if (funcThis === o2) {
    document.write('o2 <br />');
}
</code>
</pre>
