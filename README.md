# React

# JSX

JSX는 자바스크립트의 확장 문법이며 XML과 매우 비슷하게 생겼다 

JSX의 장점으로는 보기가 쉽고 익숙하며 HTML 태그와 컴포넌트도 JSX 안에서 작성할 수 있다

하지만 올바르게 사용하기 위해서는 몇 가지 규칙을 준수 하여야 한다.

### JSX 문법

컴포넌트에 여러 요소가 있다면 반드시 부모요소 하나로 감싸야 한다

![image](https://user-images.githubusercontent.com/96267331/199256806-4c9b962e-79a9-4e49-b93f-2ab80b51eaa1.png)

3가지 방식으로 묶을 수 있다.

### 자바스크립트 표현

JSX 안에서는 자바스크립트 표현식을 쓸 수 있다.  작성하기 위해서는 JSX 내부에서 코드를 {  } 감싸면 된다

![image](https://user-images.githubusercontent.com/96267331/199257056-540a256a-5f79-4e62-b469-d607b9ac8472.png)

JSX 내부의 자바스크립트 표현식에서 if 문을 사용할 수는 없다 하지만 조건에 따라 다른 내용을 렌더링 할때는 JSX 밖에서 if 문을 사용하여 사전의 값을 넣거나 {  } 안에 조건부 연산자를 사용하여야 한다. 아래의 코드는 조건부 연산자를 사용한 것이다

![image](https://user-images.githubusercontent.com/96267331/199257122-4ab5370c-350e-41b0-af13-cf6de480fcde.png)

# 컴포넌트

### props

props는 properties를 줄인 표현으로 컴포넌트의 속성을 설정할 떄 사용하는 요소 입니다

![image](https://user-images.githubusercontent.com/96267331/199257482-62186dd2-c836-4d84-a8dc-946210d9a26b.png)

![image](https://user-images.githubusercontent.com/96267331/199257540-0834f15a-dda6-4e61-9ba6-9681fe7463c9.png)

MyComponent 속성에서 name, favoriteNumber 통해 값을 받아 출력해주고 태그 사이에있는 내용을 출력해주는 children 사용해주어 출력하였다.

### state

리액트에서 state는 컴포넌트 내부에서 바뀔 수 있는 값을 의미한다 props 부모 컴포넌트가 설정하는 값이며 props 를 바꾸려면 부모 컴포넌트를 바꾸어 주어야한다 예를 들어 방금 만든 코드에서 아래쪽 컴포넌트를 통해 name 값을 받아와 사용하는데 막상 위쪽 컴포넌트에서는 전달받은 name 값을 직접 바꿀 수 없는 것을 의미한다

![image](https://user-images.githubusercontent.com/96267331/199257721-168afb4f-9346-4d2e-b925-4696cfc225a4.png)

![image](https://user-images.githubusercontent.com/96267331/199257772-86ad3e61-d0bc-468a-84be-e453f86e0dcf.png)

![image](https://user-images.githubusercontent.com/96267331/199257836-2c952731-81c8-4358-b9b4-1dc29e2c89dd.png)

state 사용해 만들어주어 위쪽 컴포넌트의 버튼을 통해서 자기 스스로 값을 바꿀수 있는 코드를 만들수 있다 그리고 위에 사용한 state는 클래스를 사용하였는데 함수를 통해 만드는 usestate 사용해 만들 수 있다

![image](https://user-images.githubusercontent.com/96267331/199258131-76ce4e8e-b425-4631-bf97-f7f75b557f96.png)

초기 상태

![image](https://user-images.githubusercontent.com/96267331/199258349-60862cd2-fc52-4094-97f8-a08b768690d8.png)

입장 클릭시<br>
![image](https://user-images.githubusercontent.com/96267331/199258469-54d67cc3-0f48-4501-8f6a-eb7bb8be89e3.png)

퇴장 클릭시<br>
![image](https://user-images.githubusercontent.com/96267331/199258528-5c9892aa-fcd7-468c-bea3-a2c8e38659f4.png)

그리고 밑의 색깔을 클릭시 글자의 색이 바뀐다.<br>

![image](https://user-images.githubusercontent.com/96267331/199258584-95473e87-5595-469e-ae3f-629531e3532c.png)

# 이벤트

이벤트는 사용자가 웹 브라우저에서 DOM 요소들과 상호작용을 하는것을 의미한다

![image](https://user-images.githubusercontent.com/96267331/199258826-654bfd9a-2069-430c-b822-9c2236e5b044.png)<br>
![image](https://user-images.githubusercontent.com/96267331/199258872-87ac770d-2a3f-4058-a9ee-a01e140386c1.png)<br>

![image](https://user-images.githubusercontent.com/96267331/199259000-c9bf4300-7bae-40af-b582-21887a0e8512.png)

# ref: DOM에 이름달기
![image](https://user-images.githubusercontent.com/96267331/199259506-ddc3ecb6-5d46-42bc-a44f-403d9112dc4a.png)<br>
![image](https://user-images.githubusercontent.com/96267331/199259616-bea20460-9423-4b4d-98bb-f0bee972e7b0.png)<br>
![image](https://user-images.githubusercontent.com/96267331/199259665-8ec3e606-c533-49a2-a93e-b4dbb0caa5d5.png)<br>
![image](https://user-images.githubusercontent.com/96267331/199259723-061ff553-24ae-4316-b8b8-6bede62beed9.png)<br>
![image](https://user-images.githubusercontent.com/96267331/199259764-a4d0c776-42b1-4c44-a08d-011c7a5392a7.png)<br>
![image](https://user-images.githubusercontent.com/96267331/199259805-b281e363-c2da-473c-bf96-d5a692453299.png)

# 컴포넌트 반복
![image](https://user-images.githubusercontent.com/96267331/199260018-7338dc30-1dc1-4791-977f-04145ca7c80f.png)<br>
![image](https://user-images.githubusercontent.com/96267331/199260054-66f2b412-1f8a-41c8-951e-bb6197656d5a.png)<br>
![image](https://user-images.githubusercontent.com/96267331/199260104-3573af99-bdb4-4bcc-8453-809365460aee.png)


