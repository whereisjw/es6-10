# var let const 선언,할당,범위

/_
var
let
const
선언 할당범위
_/

var 이름 = "kim";
var 이름 = "park";
이름 = "lee";
// 재선언이 가능함
// 재할당도 가능함
// 범위는 function

let 나이 = 20;

/_ let 나이 = 30; 에러발생_/
나이 = 40;

// 재선언이 불가
// 재할당 가능

const 나이2 = 20;

const 사람 = { 이름: "kim" };

사람.이름 = "park";
// 안에있는 object는 변경가능

//완전 변경 불가능한 변수를 만드려면 ?
Object.freeze(사람);
사람.이름 = "park2";
console.log(사람); //park 으로 출력됨

function 함수() {
var 이름3: "kim";
}
//var 은 범위가 함수이다
console.log(이름);

if (true) {
let 이름 = "park";
}

// let 과 const 는 범위가 중괄호이다
