<h1 align="center"> KB헬스케어 기업과제 </h1>
<p align="center">
  <img src="https://img.shields.io/badge/-Typescript-3178C6?style=flat-square&logo=TypeScript&logoColor=white"> <img src="https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=React&logoColor=white"> <img src="https://img.shields.io/badge/-Sass-CC6699?style=flat-square&logo=Sass&logoColor=white"> <img src="https://img.shields.io/badge/-React%20Query-FF4154?style=flat-square&logo=React%20Query&logoColor=white">
</p>

<h2 align="center"><a href="/">배포 페이지</a></h2>

# 과제 설명

## 실행 방법

## 폴더 구조

```
아직 없
```

## 구현 방법과 이유, 사용한 기술

### 맞춤 건강관리 컴포넌트

#### 데이터 정리

- 맞춤 건강관리 컴포넌트는 비슷한 모습을 하고 있어 재사용이 가능한 컴포넌트로 만들면 효율적입니다.

  - 허나 사용해야 할 데이터 객체가 매우 복잡한데다가, 데이터가 여기저기 흩어져 있었고, 배열 형식으로 되어 있지 않아 `map` 메서드를 통한 컴포넌트 재활용이 불가능했습니다.

  - 또한 몇몇 데이터는 JSON 객체 파일이 아닌 ppt 안에 정리되어 있는 등, 정돈되지 않은 데이터의 형태를 띄고 있어 활용이 어려웠습니다.

- 따라서 제일 먼저 JSON 객체 내부에서 '맞춤 건강관리 컴포넌트' 에서만 쓰는 데이터들을 추출하여 연속된 객체 배열로 만들었습니다.

  - ppt에 들어있고 JSON에 들어있지 않은 데이터도 객체 배열에 각각 넣어주었습니다.

- 데이터를 정리하고 새로운 객체 배열을 만드는 함수는 맞춤 건강관리 컴포넌트에서 사용하되, 그 길이가 매우 길어 커스텀 훅으로 분리하였습니다.

#### CSS 작업

- 제공된 SVG 파일과 ppt 예시를 참고하여 스타일링하였습니다.

- 위에서 정리한 데이터를 토대로 맞춤 건강관리 카드를 하나의 컴포넌트로 제작하여 공통 스타일링을 적용하고, 아이콘이나 색상 등 각 카드마다 다른 속성들은 클래스명 등을 이용하여 조건부 스타일링을 적용하였습니다.

- 정상범위가 존재하는 카드 (신사구체여과물 등) 와 존재하지 않는 카드 (운동량 등) 에 대해서 조건문을 통해 정상범위 문자열을 추가하였습니다.

### 건강점수 시각화

- 개인 건강 점수를 베어 문 도넛 모양으로 표시하는 부분은 svg로 그려서 구현하였습니다.

- dash array만 잘 설정하면 쉽게 구현할 수 있다고 생각하여서 svg로 만들었습니다. 

### 회원 개인 건강 정보 

- 회원의 성별, 나이, 키 값을 JSON 데이터의 구조 분해를 통해 불러와 화면에 띄워주었습니다.

- useNavigate hook을 사용하여 결과 자세히 보기 버튼 클릭 시 detail 페이지로 이동할 수 있게 구현하였습니다. 

<hr />

<h2 align="center">기여한 사람들</h2>
<p align="center">
<table align="center">
  <thead>
    <tr>
      <th><a href="https://github.com/kec0130">🌅 고은채</a></th>
      <th><a href="https://github.com/HyeongSeoku">🌇 김형석</a></th>
      <th><a href="https://github.com/lazy-sky">🌃 김하늘</a></th>
      <th><a href="https://github.com/han-byul-yang">🎇 양한별</a></th>
      <th><a href="https://github.com/yhnb3">🌠 엄강우</a></th>
      <th><a href="https://github.com/Keunyeong">🌉 이근영</a></th>
      <th><a href="https://github.com/chichoon">🏙 최지윤</a></th>
    </tr>
  </thead>
</table>
</p>
