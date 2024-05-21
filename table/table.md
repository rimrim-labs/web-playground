# 테이블 

## CSS

### border-collapse
테이블 내부 셀 간의 `border` 공유 여부를 설정한다.
- collapse
- separate

(1) `collapse`
- 이웃한 셀 간 `border`를 공유한다

(2) `separate`
- 이웃한 셀 간 독립된 `border`를 갖는다
- `border-spacing` 속성 값에 의해 셀 `border` 간격이 결정된다

### table-layout
테이블 내부 셀의 배치 방식을 설정한다.
- auto
- fixed
- inherit

(1) `auto`
- 기본값으로, 행의 너비는 셀 내부 컨텐츠 길이에 의해 결정된다
- 테이블의 모든 컨텐츠를 읽어야 레이아웃이 결정되므로 다소 렌더링이 늦어질 수 있다

(2) `fixed`
- 테이블 컨텐츠가 아닌 지정된 `width` 속성 값에 의해 행 너비가 결정된다
- 테이블 컨텐츠와 상관없이 렌더링 가능하므로 `auto` 보다 속도가 빠르다

각 행의 너비는 아래와 같은 우선순위에 의해 결정된다
- `col`에 설정된 `width` 값
- 명시적으로 `width`가 설정된 첫 번째 행의 너비 값
- 남는 공간 내에서 적절한 너비 값