# @keyframes

- `@keyframes` CSS에서 애니메이션을 작성하기 위해 사용하는 쿼리로, `from`부터 `to`까지 혹은 `0%`부터 `100%`까지, 애니메이션의 한 사이클에 대한 내용을 담는다.
- 작성 예시는 아래와 같다.
   > ```css
   > @keyframes [애니메이션 이름] {
   >     from {
   >     }
   >     to {
   >     }
   > }
   > ```

# animation-delay

- `animation-delay` 속성은 애니메이션의 최초 사이클이 시작되기 전 지연시킬 시간을 지정한다. 사이클 간의 시간에는 영향을 미치지 않는다.
- 값
  - 시간 값 

# animation-duration

- `animation-duration` 속성은 한 사이클을 완성하는데 걸리는 시간을 지정하기 위한 속성이다.
- 값
  - 시간 값 

# animation-iteration-count

- `animation-iteration-count` 속성은 애니메이션 반복 횟수를 지정하기 위해 사용한다.
- 값  
  - 자연수: 기본값은 `1`이다.
  - `infinite`: 무한히 반복한다.

# animation-name

- `animation-name` 속성은 `@keyframes` 쿼리에서 작성한 `애니메이션 이름`을 값으로 사용하여 선택자에 의해 선택된 요소에 애니메이션을 적용하기 위한 속성이다.
- 값
  - `none`: _[기본값]_ 애니메이션 없음
  - 애니메이션 이름

# animation-play-state

- `animation-play-state` 속성은 애니메이션 재생 상태를 지정하기 위한 속성이다.
- 값
  - `running`: _[기본값]_ 재생 중
  - `paused`: 일시 정지

# animation-timing-function

- `animation-timing-function` 속성은 애니메이션이 적용되는데 있어, 시간의 흐름에 따른 사이클 완료율을 계산하는 함수를 지정하기 위한 속성이다.
- 값
  - `ease`: _[기본값]_
  - `ease-in`
  - `ease-in-out`
  - `ease-out`
  - `linear`
  - `cubic-besizer` 함수: 사용자 정의 베이저 곡선 함수
- 참고: https://matthewlein.com/tools/ceaser