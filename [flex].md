# [flex]

- 플렉스 컨테이너는 이가 가지는 자식 요소들에 대한 배치를 보다 유연하고 쉽게하기 위해 사용한다.
- 플렉스 컨테이너가 될 요소의 `display` 속성 값을 `flex` 혹은 `inline-flex`로 설정한다.

## 플렉스 컨테이너(부모)

### align-items

- `align-items` 속성은 플렉스 컨테이너의 `flex-direction`에 대해 **수직한 방향**으로의 정렬을 위한 속성이다.
- 값
  - `flex-start`: 흐름 방향에서 시작하도록 정렬.
  - `flex-end`: 흐름 끝 방향에서 시작하도록 정렬.
  - `center`: 가운데 정렬.
  - `space-between`: 각 플렉스 아이템의 사이에 균등한 공간을 배분한다.
  - `space-around`: 각 플렉스 아이템의 사이에 균등한 공간을 배분하고, 각 끝 아이템의 외부 여백 또한 배분하는데, 외부 여백은 각 플렉스 아이템 사이 여백의 절반이다.
  - `space-evenly`: 각 플렉스 아이템의 사이 및 각 끝에 균등한 공간을 배분한다.
  - `stretch`: 플렉스 컨테이너의 크기에 맞게 늘이거나 줄인다.

### flex-direction

- `flex-direction` 속성은 플레스 컨테이너에 부여하는 속성으로, 이가 포함하고 있는 아이템들의 흐름 방향을 지정하기 위해 사용한다.
- 값
  - `row`: _[기본값]_ 가로 방향.
  - `row-reverse`: 가로 역방향. 요소의 순서도 함께 반전됨에 유의.
  - `column`: 세로 방향.
  - `column-reverse`: 세로 역방향. 요소의 순서도 함께 반전됨에 유의.

### gap

- `gap` 속성은 플렉스 컨테이너가 포함하는 아이템간의 거리를 지정하기 위해 사용한다.
- 형태
  - `[값1]`: `값1`이 크기 값일 때, 행간, 열간 거리를 모두 `값1`로 지정한다. 
  - `[값1 값2]`: `값1`과 `값2`가 크기 값일 때, 행간 거리를 `값1`로, 열간 거리를 `값2`로 지정한다.

### justify-content

- `justify-content` 속성은 플렉스 컨테이너의 `flex-direction`에 대해 **수평한 방향**으로의 정렬을 위한 속성이다.
- 값
  - `flex-start`: 흐름 방향에서 시작하도록 정렬.
  - `flex-end`: 흐름 끝 방향에서 시작하도록 정렬.
  - `center`: 가운데 정렬.
  - `space-between`: 각 플렉스 아이템의 사이에 균등한 공간을 배분한다.
  - `space-around`: 각 플렉스 아이템의 사이에 균등한 공간을 배분하고, 각 끝 아이템의 외부 여백 또한 배분하는데, 외부 여백은 각 플렉스 아이템 사이 여백의 절반이다.
  - `space-evenly`: 각 플렉스 아이템의 사이 및 각 끝에 균등한 공간을 배분한다.

## 플렉스 아이템(자식)

### flex

- `flex` 속성은 `flex-basis`, `flex-grow`, `flex-shrink` 세 가지 속성의 축약 속성이다.
- 형태
  - `[flex-basis 값] [flex-shrink 값] [flex-grow 값]`
    > ```css
    > * {
    >     flex: 0 0 auto;
    > }
    > ```
    > - 위 속성은 아래와 같다.
    > ```css
    > * {
    >     flex-basis: auto;
    >     flex-grow: 0;
    >     flex-shrink: 0;
    > }
    > ```

### flex-basis

- `flex-basis` 속성은 플렉스 아이템의 초기 크기를 지정하기 위해 사용한다.
- 플렉스 컨테이너의 `flex-direction` 속성 값이 `row`일 때 이는 `width`와 동일하며, `column`일 때 이는 `height`와 동일하다.
- 값
  - `auto`: _[기본값]_ 요소가 가지는 내용에 따라 자동 조절.
  - 크기 값

### flex-grow

- `flex-grow` 속성은 플렉스 아이템이 플렉스 컨테이너 안에서 `flex-direction` 방향에 따라 남는 여유 공간을 차지하기 위해 늘어날 비율을 지정한다.
- 값
  - `0`이상의 정수: 기본 값은 `0`이다. 

### flex-shrink

- `flex-shrink` 속성은 플렉스 아이템이 플렉스 컨테이너 안에서 `flex-direction` 방향에 따라 줄어들 비율을 지정한다. 단, 이가 가진 내용을 표시하기 위한 최소한의 크기 미만으로 줄지 않는다.
- 값
  - `0`이상의 정수: 기본 값은 `1`이다. 