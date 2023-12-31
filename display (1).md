# display

- `display` 속성은 요소가 표시될 방식을 지정하기 위한 속성이다.
- 값
  - `block`: 해당 요소를 포함하고 있는 부모 요소의 줄 전체를 차지하는 플로우 컨텐츠. `<div>`, `<section>`, `<header>` 태그 등이 이에 속한다. 
  - `inline`: 텍스트의 흐름에 포함되는 구문 컨텐츠. `<a>`, `<b>`, `<span>` 등이 이에 속한다. 단, `display` 속성 값이 `inline`인 태그는 크기 설정(`width`, `height`)이 불가하다. 
  - `inline-block`: `inline`의 속성을 가지는 구문 컨텐츠이면서 크기 설정 등이 가능하도록 일부 `block`의 속성도 가지는 속성 값.
  - `none`: 요소를 표시하지 않는다. 크기 또한 차지하지 않게된다.
  - `flex`: 해당 요소를 플로우 컨텐츠형 플렉스 컨테이너로 표시한다.
  - `inline-flex`: 해당 요소를 구문 컨텐츠형 플렉스 컨테이너로 표시한다.
  - `grid`: 해당 요소를 플로우 컨텐츠형 그리드 컨테이너로 표시한다.
  - `inline-grid`: 해당 요소를 구문 컨텐츠형 그리드 컨테이너로 표시한다.