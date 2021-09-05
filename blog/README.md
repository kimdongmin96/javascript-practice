# React Practice

### react 실습
<br>
react를 사용 시 데이터바인딩이 간편해진다. <br>

```javascript
<h1>안녕하세요</h1>
```

hello 변수에 안녕하세요를 저장 후 

```javascript
<h1> { hello } </h1>
```

<hr>
자주 변경되는 데이터는 useState로 정의<br>

```javascript
let [a, b] = useState('안녕하세요');
```

변수 a에는 '안녕하세요' 문자열이 저장되고 변수 b는 a를 변경하는 함수가 저장된다.<br>
a를 변경할 때 b(변경내용) 형식으로 변경

