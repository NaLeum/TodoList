바닐라 자바스크립트 : 자바스크립트 중에 라이브러리가 없는 자바스크립트
javascript : 언어
ECMAScript ; Specification의 명칭
Specification : 안내 책자, 안내문, 설명문

자바스크립트는 못생겼다. 
why? 온갖 임시방편과 떼운것들로 더렵혀져있기 떄문이다. 

라이브러리와 프레임워크는 화장같은것이다.
    자바스크립트를 원래모습보다 좀 더 예쁘게 만들어 주는것.

변수 variable : 변할수있는 값
    1. Create 생성
    2. Initialize 초기화
    3. Use 사용

    let 변해도 되는 값 덮어쓰기 가능
    const constant(상수) 절대로 변하면 안되는 값

    첫사용은 const 필요할떄만 let

Array 배열 : 데이터를 저장하는 곳, 리스트 같은것
    const daysOfWeek = ["Mon","Tue","Wed","Thu","Fri","Sat","Sun"];

Object 객체 : 각 value에 이름을 붙여줄 수 있다.
    const naleumInfo = { name : "NaLeum", age : 26, gender:"Male"};

console.log == console은 자바스크립트의 object이다. 
    console이라는 object의 log의 이름을 가진 value를 보여줘
    ==bulit-in-function

function : 함수
    function sayHello(){
        console.log("Hello");
    }

    sayHello();

    function sayHello(parameter){
        console.log('Hello', parameter);
    }
    sayHello("Hi");

자바스크립트에서는 ''도 스트링 ""도 스트링이다. 

섹시하게 콘솔로그를 찍어보자
    function sayHello(name, age){
        console.log(`Hello $(name) you are $(age) years old`);
    }
    
    sayHello("Naleum",15);

return : 거스름돈 같은 것
    function sayHello(name,age){
        return `Hello $(name) you are $(age) years old`;
    }

    consy greetNaleum = sayHello("Naleum",26);

    console.log(greetNaleum);

    -
    const calculator = {
        puls : function(a,b){
            return a + b;
        }
        
        minus : function(a,b){
            return a - b;
        }
        곱하기 : function(a,b){
            return a * b;
        }
        나누기 : function(a,b){
            return a/b;
        }
        제곱 : function(a,b){
            return a ** b;
        }
        나머지 : function(a,b){
            return a % b;
        }

    }

    const plus = calculator.plus(5,5);
    console.log(plus);


DOM 자바스크립트는 도큐먼트=html를 객체로 만들꺼야 