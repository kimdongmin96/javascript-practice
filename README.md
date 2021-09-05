# javascript-practice

### Selector
```
document.getElementById('@').??? = ???;
document.querySelector('@').??? = ???;
```
'@'에 해당하는 ID(querySelector는 css선택자)를 찾고 '?'에 해당하는 일을 처리하는 작업   
*ex) innerHtml을 통해 html 내용 변경*
***
### function
함수를 통해 장문의 코드를 간단하게 사용 가능
```
<div id='box'>박스</div>
<button onclick="document.getElementById('box').innerHtml = '박스변경'">버튼</button>
```
해당 코드를 사용하면 html 내의 내용이 복잡해진다. 이를 함수를 이용하여 변경하면
```
<div id='box'>박스</div>
<button onclick=내용변경()>버튼</button>
.
.
<script>
  function 내용변경() {
    document.getElementById('box').innerHtml = '박스변경';
  }
</script>
```
반복적인 작업에서 매개변수를 활용한다면 html 재활용 등 다방면으로 사용 가능
***
### 이벤트리스너 & jQuery
버튼의 onclick를 이벤트리스너를 통해 변경 가능
```
<button id='btn'>버튼</button>
.
.
<script>
  document.getElementById('btn').addEvemtLinstener('click', function() {
    처리 내용
  }
</script>
```
jQuery 이용 시   
**document.getElement.... -> $('#...').???** (여기서 '#'을 사용하면 id값, '.'을 사용하면 class값)
