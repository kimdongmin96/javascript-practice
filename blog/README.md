# React Practice

### react를 사용 시 데이터바인딩이 간편해진다.

```javascript
<h1>안녕하세요</h1>
```

hello 변수에 안녕하세요를 저장 후 

```javascript
<h1> { hello } </h1>
```

<hr>

### 자주 변경되는 데이터는 useState로 정의

```javascript
let [a, b] = useState('안녕하세요');
```

변수 a에는 '안녕하세요' 문자열이 저장되고 변수 b는 a를 변경하는 함수가 저장된다.<br>
a를 변경할 때 b(변경내용) 형식으로 변경<br><br>
useState 사용 시 변수를 직접적으로 바꿔주는 것은 좋지 않다.<br>
재랜더링이 되지 않을 수 있다.<br>
예를 들어,

```javascript
let [글제목, 글제목변경] = useState(['남자 코트 추천', '강남 우동맛집', '파이썬독학']);

function 제목바꾸기(){
  var newArray = [...글제목];
  newArray[0] = '여자 코트 추천';
  글제목변경(newArray);
}
```

새로운 변수를 생성 후 deep copy를 통해 '글제목' 값을 저장한 후 '글제목변경' 함수를 통해 내용을 바꿔준다.
<hr>

### component 사용


