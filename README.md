#  스터디


1. next.js를 왜 쓰는가?
    - 고객 유입을 위한 SEO 최적의 리액트 프레임워크이기 때문에 고객의 유입이 많아져야 하는 스타트업의 회사가 이 프래임 워크를 많이 사용한다고 한다. 리액트로도 안되는건 아니다 그래서 섞어서 쓰는것.
 
스타트업일 아닐경우에는 고객을 상대하는게 아니기 떄문이기도하고 기존의 레거시도 유지보수 해야하기 때문에 next.js를 쓰지 읺는 이유도 있다.  
 
2. 리액트 강의 3년 전꺼는 봐도 되는가?
    - 업데이트가 되었다고 해도 기존거를 최신으로 바꾸기 힘들고 에러가 어디서 터질지 모르는 거이기 때문에
기본은 알아야한다.
 
3. null과 undefinde를 언제 쓰는가?
    API를 받아서 쓸 때 데이터에 값이 있는 것과 값이 없는것이 있는데 null이었을 때 사용자에게 어떤 화면을 보여주는지 삼합연산자를 사용해서 화면에 보여 준다고 한다.


<img width="80%" src="https://github.com/Katie27-maker/fe-fronStudy/assets/59760987/8c4ac2ba-2678-4aae-9473-1d2d94d9dd10"/>

---------------------------------------------------------------------------------------------------------------------------------------------------------------------

![스크린샷 2024-04-13 오후 11 54 12](https://github.com/Katie27-maker/React-fronStudy/assets/59760987/f4526b66-55ee-4910-bc85-feb2d2011857)

import React, { useState } from "react";

const Home = () => {
  const [setData, setDataText] = useState("요기");

  const [showText, showDataText] = useState("");

  const 함수임 = (props) => {
    setDataText(props.target.value);
  };

  const 클릭임 = () => {
    showDataText(setData);
  };

  return (
    <div>
      <div>{showText}</div>

      <input type="text" onChange={함수임} placeholder="입력 ㄱ ㄱ "></input>
      <button onClick={클릭임}>클릭하셈</button>
    </div>
  );
};

export default Home;

