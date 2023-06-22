## React
```
JSX {} means JS Area
```
### 랜더링 기준
```
state의 변경
props의 변경
부모 자식간의 컴포넌트 변경
context의 변경
```
### React Hook
```
useState 는 변수를 제어하는 훅으로 re render를 하게해줌
useEffect 는 mount에서 작동하는 훅
useContext는 값을 전역으로 사용하게 해주는 훅
useReducer는 useState를 외부로 빼낸 버전
useCallback은 함수에 대한 메모지네이션
useMemo는 컴포넌트에 대한 메모지네이션
```
### Redux
```
* 리덕스 3대 요소
Action - final Value
type - 생성자(인자값 형태 정의) , dispatch에 들어가는값 -> 한마디로 기준값이라고 생각
Reducer - function 이고 , payload에 type에 들어온값이 들어옴
* https://nyang-in.tistory.com/247 참고

* dispatcher가 type을 reducer에 넣어준다
redux duck pattern - 효율적 패턴
redux action handleAction lib는 type생성자 자동화, 파라미터 payload자동화를 해준다
```
<hr/>

## Vue Main Concept

### Vuex
```
helper
```

### Derectory Folder
```
Api
Store
plugIn
View
Asset
```
### Cycle
```
watch
filter 
mounted
async create 
function
```

### Reference
```
https://redux.vlpt.us/4-2-redux-actions.html
```


