JSX 문법


규칙 
1. 속성명은 카멜케이스로 작성하기(ex. onClick)
2. 자바스크립트 예약어와 같은 속성명은 사용할 수 없다.
3. 반드시 하나의 요소로 감싸기 - Fragment
4. 자바스크립트 표현식 넣기

위와 같은 규칙을 잘 적용하면

import ReactDOM from 'react-dom';

const product = 'Macbook';
const model = 'Air';
const imgurl = 'https://-';

function handleClick(e) {
    alter('곧 도착합니디');
}

ReactDOM.render(
    <>
     <h1>{product+ ' ' + model} 주문하기</h1>
     <img src={imgurl} alt='제품 이미지'/>
     <button onClick={handleClick}>확인</button>
    </>
) 