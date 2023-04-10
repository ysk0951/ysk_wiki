## 개인앱 비즈니스모델 구축및 구현

### 앱 프로젝트 홍보기획
```
😀 린 비즈니스의 특성상 홍보수단부터 구성
고객의 앱/웹 서비스를 선택하여 자동적 바이럴을 일으키도록 유도 (제로마케팅이 효과적)
ex) 공유버튼에 의한보상, 친추를 초대하지 않을경우 게임의 횟수 제한등
Apply) 유기견 후원시스템 개발 -> 제로마케팅 적용
```
### 앱 구현
```
😀 가장 적고 즉각적인 기능으로 구현
기능이 복잡해지고 최종적인 return을 받기까지 흐름도가 길면 서비스의 브랜드 퀄리티가 떨어짐
단순기능으로도 Service의 아이덴 티티가 명확해야함
기능상 승수효과를 누릴수있는 포인트를 넣어놔야 홍보기획이 의미가 있음
Apply) 유기견 신고 프로세스를 MVP로 개발
```
### 기술선택 
```
최대한 빠르게 생산성에 집중
잘된코드, 유지개발이 용이한 코드를 위해 코드를 세부적으로 쪼개거나 디렉토리의 볼륨을 키우는것은 의미가 없음
피드백이 가장 중요하기때문에 선출시후 리펙토링을 하는 애자일 방식을 선택
Apply) 크로스플랫폼 언어인 React Native를 선택, 랜더링 페이지의 형태를 띄며 조금 발전할경우 가장작은 단위의 AWS선택
```
### 수익모델
```
고객경험을 강화하거나, 침해하지않는 수익모델을 적용
😀 AdMob , 개발자 후원시스템 , 정부사업지원금
Apply) 유기견 후원시스템, 유기견 정부사업 지원
```
### Reference
```
😀 Dev Enviroment
https://dev-yakuza.posstree.com/ko/react-native/install-on-mac/
https://velog.io/@jeon_131/React-Native-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8-%EB%A7%8C%EB%93%A4%EA%B8%B0
https://talkwithcode.tistory.com/45?category=1036047
https://github.com/facebook/react-native/issues/28712
https://zionh.tistory.com/28
https://defineall.tistory.com/1151
https://medium.com/nextunicorn/%EC%95%88%EB%85%95%ED%95%98%EC%84%B8%EC%9A%94-nextunicorn-%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4-%EC%97%94%EC%A7%80%EB%8B%88%EC%96%B4-mino-%EC%9E%85%EB%8B%88%EB%8B%A4-2678dd0a4af4
https://m.blog.naver.com/PostView.naver?blogId=zion830&logNo=221353306321&proxyReferer=
https://velog.io/@dody_/RN-Library-%EB%A6%AC%EC%95%A1%ED%8A%B8%EB%84%A4%EC%9D%B4%ED%8B%B0%EB%B8%8C-%EB%94%94%EB%B2%84%EA%B1%B0-%EB%8F%84%EA%B5%AC-react-native-debugger-redux-devtools-react-native-debugger-open
https://medium.com/duckuism/react-native-%EB%94%94%EB%B2%84%EA%B9%85-%ED%99%98%EA%B2%BD-%EB%A7%8C%EB%93%A4%EA%B8%B0-7e46bfe89f6
https://reactnativeelements.com/
https://memostack.tistory.com/53
```