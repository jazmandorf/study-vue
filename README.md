# study-vue
study vue.js
start project Nov.17 2018


#Vue js
</hr>
## 인스턴스와 컴포넌트
인스턴스와 컴포넌트가 있다.
인스턴스는 하나의 레고로 치면 레고를 쌓을수 있는 판이라고 생각하면 된다.
그리고 컴포넌트 레고 하나하나의 블럭이라고 생각하면 될 것 같다.

우리가 보통 웹페이지를 헤더, 바디, 푸터 이렇게 만든다고 했을때
각각의 헤더, 바디, 푸터 가 컴포넌트가 된다고 생각하면 될 것같다.
컴포넌트도 변수 처럼 전역과 지역 변수를 선언할 수 있으며
전역으로 선언할 때에는
<pre><code>Vue.component('컴포넌트 네임',{template : '', props : ['']})</code></pre>
지역으로 선언할 떄에는 인스턴스 안에
components라는 항목으로 추가해 주면 된다.
인스턴스 안에서 함수로 data 값을  return 하고자 할때에는
<pre><code>data : ()=>{
    var return_data = 'return data';
    return {return_data,  return_data2 : 'returndta2'} // 이런식으로 여러 값도  return 해줄 수 있다.
}</code></pre>

## v-bind
특징 : 다른 곳에서 쓰인 변수가 값들을 가져와서 묶어줄떄 사용하면 된다라고 이해함.
속성 props 을 정의할때 대문자와 - 가 들어가면 안됨 언더바는 되드라.
컴포넌트에는 배열로 대괄호로 막아서 써 주어야 함.[]
v-bind:props = 'message'
이렇게 하면  인스턴스가 부모가 되고 셋팅한 전역 컴포넌트가 자식이 되어서
인스턴스에서 선언한 데이타 값을 받아서 사용할 수 있게된다.

by Jaz

