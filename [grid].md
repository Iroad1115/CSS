# [grid]

- 그리드 컨테이너는 이가 가지는 자식 요소(그리드 아이템)들에 대한 반복되는 격자 배치를 보다 쉽게하기 위해 사용한다.
- 그리드 컨테이너가 될 요소의 `display` 속성 값을 `grid` 혹은 `inline-grid`로 설정한다.

## 그리드 컨테이너(부모)

### grid-template-columns

- `grid-template-columns` 속성은 그리드 컨테이너에 부여하는 속성으로, 그리드의 열의 구조를 설정하기 위한 속성이다.
- 값
  - 크기 값
  - `fr` 값
- 형태
  - `[값 ...]` 

###  grid-template-rows

- `grid-template-rows` 속성은 그리드 컨테이너에 부여하는 속성으로, 그리드의 행의 구조를 설정하기 위한 속성이다.
- 값
  - 크기 값
  - `fr` 값
- 형태
  - `[값 ...]`

### gap

- `gap` 속성은 그리드 컨테이너가 포함하는 아이템간의 거리를 지정하기 위해 사용한다.
- 형태
  - `[값1]`: `값1`이 크기 값일 때, 행간, 열간 거리를 모두 `값1`로 설정한다.
  - `[값1 값2]`: `값1`과 `값2`가 크기 값일 때, 행간 거리를 `값1`로, 열간 거리를 `값2`로 설정한다.

## 그리드 아이템(자식)

### grid-column

- `grid-column` 속성은 해당 아이템이 차지해야하는 열의 번호를 지정하기 위해 사용한다.
- 형태
  - `[시작 번호] / [끝 번호]`
  - 슬래쉬(`/`)의 좌우에는 반드시 공백이 있어야 함에 유의한다.

### grid-row

- `grid-row` 속성은 해당 아이템이 차지해야하는 행의 번호를 지정하기 위해 사용한다.
- 형태
  - `[시작 번호] / [끝 번호]`
  - 슬래쉬(`/`)의 좌우에는 반드시 공백이 있어야 함에 유의한다.

### order

- `order` 속성은 해당 아이템의 태그 순번과 관계 없이, 시각적으로 배치되어야 하는 순서를 지정하기 위해 사용한다.
- 단, `grid-column`, `grid-row` 속성이 적용되어 있다면 `order` 속성은 무시된다.
- 속성 값이 같은 아이템끼리는 태그의 배치 순서에 따라 표시된다.
- 값
  - `[정수]`: 숫자가 작을수록 우선 배치된다. 기본값은 `0`이다. 