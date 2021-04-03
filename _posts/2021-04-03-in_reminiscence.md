---
layout: post
title:  "Full Pre 수료 / Codestates 회고"
categories: CodeStates
---

하루하루 정신없이 지내다 보니 어느덧 Full Pre 코스 부분을 수료했다.. 시간이 엄청 빨리 지나간 것 같다.  
그동안 같이 공부하신 기수 동기분들과 열심히 멘토 역할을 해주신 분들도 정말 고생하셨고 참으로 감사드린다.  
4주라는 짧은 기간 동안 정말 많은 것들을 배웠다. 배우고 끝나버리면 잊어버리기 쉬울 것 같아 지난 배운 것들을 기억하며 정리해보는 시간을 가지려 한다.  

*~~아직 개발자가 되기위해 배우는 과정이기 때문에 잘 못 알고있는 부분이 많지만 보완하려 노력해야겠다. 따라서... 잘못 이해하고 적고있을 수도 있다...~~*

---
## 1주차
1주차에는 js의 기본적인 부분들... 변수선언, 함수, 조건문, 문자열, 반복문에 대해서 배우는 시간을 가졌다. 그리고 HTML과 css의 기초적인 부분도 배웠다.

먼저, 변수라 함은 이름 같은 것인데 var, let, const 등등 이러한 것들로 변수를 새로 선언해줘야한다.
``` js
var = x;
let = y;
const = z;
```
>var는 선언과 할당의 제한이 없다. 선언의 제한이 없기 때문에 코딩을 할 때, 같은 이름의 변수가 계속 선언되기 때문에 사용을 지양한다.  
>let은 할당의 제한이 없지만 선언은 한번밖에 되지 않는다. 그러기 때문에 var의 단점을 보안한 변수선언이라고 볼 수 있다.  
>const는 선언과 할당의 제한을 가진다. 즉, 선언과 할당을 한번밖에 하지 못해 주로 함수를 선언할때 쓰인다.

함수는 수학적의미의 함수와 같다고 보면된다. 함수 선언에는 함수 선언식과 함수 표현식이 있다.
``` js
funcion func() {
  consol.log('함수 선언식');
}
const func() = function () {
  consol.log('함수 표현식');
};
```
>함수 선언식과 함수 표현식의 차이는 호이스팅과 연관이 있다.  
>함수 선언식은 호이스팅의 영향을 받지만, 함수 표현식은 호이스팅의 영향을 받지않는다.  
>함수 선언식은 코드의 위치와 상관없이 호이스팅의 영향을 받아 js가 실행될때 코드의 맨위로 옮겨져 실행된다.  
>처음에 호이스팅의 개념을 이해하기 어려워 골치가 아팠다...

조건문은 if문과 while문 등이 있다.
``` js
if('조건') {
  consol.log('조건이 true라면 실행');
}
while('조건') {
  consol.log('조건이 true일때까지 실행');
}
```
>if문은 '조건' === true 라면 if문 안이 한번 실행된다.  
>while문은 '조건' === true 일때까지 while문 안이 계속 실행된다.

문자열은 말그대로 그냥 문자다...ㅋ..
``` js
let str = '문자열';
```
>문자열은 문자열의 속성과 메소드를 활용하여 많은 것들을 할 수 있다.  
>length, concat(), indexOf() 등등...  
>다양한 메소드와 활용법은 [MDN String.prototype](https://developer.mozilla.org/ko/docs/conflicting/Web/JavaScript/Reference/Global_Objects/String) 이 사이트를 참고하면 된다.

반복문은 for문이 있고, 반복문인 while문으로도 활용할 수 있다.
``` js
for('초기값'; '조건문'; '실행') {
  consol.log('초기값이 조건문에 해당할 때까지 실행문에 따라 실행.');
}
for(let i in '변수') {
  consol.log('i === 변수의 속성값(?)');
}
for(let i of '변수') {
  consol.log('i === 변수');
}
```
>for문은 초기값을 가진 새로운 변수가 필요하다. i가 '조건문' === true 일 때까지 '실행' 부분에 따라 반복된다.  
>for...in 과 for...of는 나중에 알게된 부분이지만 여기에 같이 쓴다.  
>for...in은 각 변수의 모든 속성값을 가지고 오기때문에 배열안의 객체인 변수일때 사용하면 용이하다.  
>for...of는 for문의 줄임말과 같다.  

HTML과 css는 VScode를 설치하여 간단한 기초적인 부분을 습득했다.  
우리가 앞으로 쓸 VScode를 설치하고 그 안에 편리한 extensions를 설치했다.  
여러 익스텐션을 깔았는데 아직까지도 숙달이 안됐다.. 디버그도 완벽히 활용을 못하고있다...

---
## 2주차
2주차에는 1주차때 배웠던 HTML과 css를 활용하여 calculator를 구현해보는 시간을 가졌다. js의 배열, 객체, 변수의 데이터형, 스코프의 개념에 대해 배웠고, 와이어프레임 설계 방법과 twittler를 하드코딩해보는 시간을 가졌다.

[Calculator](https://github.com/lhb7021/pre-sprint-calculator)구현은 그리 어렵지 않았다. 물론 처음이라 가이드라인이 있었기에 어렵게 느껴지진 않았던 것 같다.  
모든게 처음이라 엄청 뒤죽박죽이기는 하지만 js와 css를 활용하여 프로그램을 구현한다는게 신기했고 재밌었다.
![image](https://user-images.githubusercontent.com/79880529/113480351-dbfe9300-94ce-11eb-9710-b33c02518cdf.png){: width="300px", height="450px" }

베열은 문자열을 각각의 공간으로 배정된 저장소라고 생각하면된다.
``` js
let arr = ['one', 'two', 'three'];

consol.log(arr); // ["one", "two", "three"]
```
>배열도 배열의 속성과 메소드를 활용하여 할 수 있다.  
>[MDN Array](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Array)이 사이트를 참고하여 메소드들의 활용 방법을 알 수 있다.  

객체는 배열과 다르게 {} curly brackets를 활용하여 속성과 값을 저장하는 역활을 한다.  
``` js
let obj = {
  key: 'value'
};
consol.log(obj.key) // "value"
```
>객체 또한 객체의 속성과 여러 메소드를 활용하여 많은 작업을 할 수 있다.  
>[MDN Object](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Object)  

변수는 크게 원시 자료형(primitive data types)과 참조 자료형(reference data types)로 나뉜다.  
>원시 자료형(primitive data types)는  
>객체가 아니면서 method를 가지지 않는 6가지의 타입을 말한다.  
>string, number, bigint, boolean, undefined, symbul, (null)이 있다.  
>원시 자료형은 과거, 데이터 저장소의 용량이 제한되어 하나의 변수에는 제한된 공간이 할당되어 하나의 데이터만 들어갈 수 있었다.  
>그래서 말 그대로 원시적인 데이터라고 하는 것이다.  죽, 하나의 변수에 하나의 데이터만 넣을수 있는 타입을 원시 자료형이라고 한다.
>반면에 원시 자료형이 아닌 모든것을 참조 자료형이라 하는데,  
>참조 자료형(reference data types)는  
>배열(string)과 객체(object), 함수(function)가 대표적으로, 하나의 공간에 하나의 데이터가 들어가는 것을 공간적으로나 비용적으로 매우 비효율 적이다.  
>그래서 각 데이터의 주소값을 활용하여 데이터를 효율적으로 활용한다.
``` js
let a = [1, 2, 3];
let b = a;
b[0] = 4;
consol.log(a); // [4, 2, 3]
```
>변수 a에 데이터가 들어가는게 아니라 데이터의 주소값이 들어가기 때문에 변수 b에 변수 a의 값을 넣고, 변수 b를 수정하면 주소값이 변경되어서 변수 a의 값도 변한다.  

스코프는 해당 변수가 활동 할 수 있는 범위를 말한다. 전역변수(Global Valiable)과 지역변수(Local Valiable)로 나뉜다.  
>전역변수는 말그대로 스크립트 전체에서 쓰일 수 있는 변수라고 하고,  
>지역변수는 선언된 함수 내에서만 쓰일 수 있는 변수라고 한다.  
>여기에서 클로저 함수가 나오는데,  
>함수안에 함수를 선언할때, 외부함수의 변수를 사용 할 수 있는 내부함수를 클로저 함수라고 한다.  
``` js
function outerFn() {  //외부함수.
  let outerVar = 'outer';  //지역변수.
  function innerFn() {  //내부함수, 클로저 함수.
    let innerVar = 'inner';  //지역변수.
  }
}
let globalVar = 'global';  //전역변수.
```

와이어프레임은 HTML를 구현하기전 기초 골격을 구상해 보는 작업이다. 코딩으로 치면 알고리즘을 짜는 것과 같다.  
>와이어프레임은 종이에 직접 작성하며 구상해보는 것도 좋고 [Figma](https://www.figma.com/) 사이트를 이용해서 구상해도 좋다.  

지금까지 배웠던 css와 js를 가지고 twittler를 구현해 보는 시간을 가졌다.  
[twittler](https://github.com/lhb7021/pre-sprint-twittler)
>하드코딩으로 끝나지 않고 버튼을 누르면 스크립트가 실행되게 구현해 보았다.  
>나는 js는 정말 재밌게 배웠는데, css는 배우는데 힘들었다... 어렵거나 그런것은 아니지만... 창작의 고통같은...? 디자인을 너무 못한다..ㅠ  
![image](https://user-images.githubusercontent.com/79880529/113483124-d14afa80-94dc-11eb-95d8-e11366aff3ff.png){: width="300", height="450" }
