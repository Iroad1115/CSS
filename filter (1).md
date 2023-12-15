# filter

- `filter` 속성은 흐림이나 색상 변형 등 그래픽 효과를 적용하기 위한 속성이다.
- 속성 값은 함수로 이루어져있고 공백으로 구분하여 여러개 사용할 수 있다.
- 값
  - `none`: _[기본값]_ 없음
  - `blur(x)`: 크기 값인 `x`만큼을 반경으로 하여 요소를 흐린다.
  - `brightness(x)`: 비율 값인 `x`만큼 명도를 지정한다. `100%`(혹은 `1.0`)이 본래 명도이고, `0%`(혹은 `0.0`)으로 지정할 경우 완전히 어두워진다.
  - `contrast(x)`: 비율 값인 `x`만큼 대비를 지정한다. `100%`(혹은 `1.0`)이 본래 대비이고, `0%`(혹은 `0.0`)으로 지정할 경우 완전히 회색이 된다.
  - `grayscale(x)`: 비율 값인 `x`만큼 흑백으로 지정한다. `x`의 범위는 `0%`(혹은 `0.0`)부터 `100%`(혹은 `1.0`)까지이고, `0%`가 본래 이미지이며, `100%`가 완전한 흑백 이미지이다.
  - `hue-rotate(x)`: 각도인 `x`만큼 색조를 회전한다. `x`의 범위는 `0deg`부터 `360deg`까지이고, `360deg`를 초과할 경우 `0deg`부터 다시 순환한다. 
  - `invert(x)`: 비율 값인 `x`만큼 색상을 반전한다. `x`의 범위는 `0%`(혹은 `0.0`)부터 `100%`(혹은 `1.0`)까지이고, `0%`가 본래 이미지이며, `100%`가되면 완전히 반전된 이미지가 된다.
  - `opacity(x)`: 비율 값인 `x`만큼 불투명도를 지정한다. `x`의 범위는 `0%`(혹은 `0.0`)부터 `100%`(혹은 `1.0`)까지이고, `100%`가 본래 이미지이며, `0%`가되면 완전히 투명해 진다.
  - `saturate(x)`: 비율 값인 `x`만큼 채도를 지정한다. `100%`가 본래 채도이며, `0%`로 지정할 경우 채도가 없는 이미지가 된다.
  - `sepia(x)`: 비율 값인 `x`만큼 세피아톤을 지정한다. `x`의 범위는 `0%`(혹은 `0.0`)부터 `100%`(혹은 `1.0`)까지이고, `0%`가 본래 이미지이며, `100%`가되면 완전히 세피아톤이 된다.