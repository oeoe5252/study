# ara

## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn serve
```

### Compiles and minifies for production
```
yarn build
```

### Lints and fixes files
```
yarn lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).


### history API
```
# history.pushState
--주소 목록에 새로운 주소를 추가한다. 이전 주소가 남아있기 때문에 뒤로가기가 가능하다.
--페이지를 reload하지 않고 url만 변경해야 할 경우 사용

--history.pushState( state, title, url )
----state : 바뀐 주소와 함께 저장할 데이터 객체
----title : 바꿀 제목
----url   : 바꿀 주소. 지정하지 않은 경우 문서의 현재 URL을 사용



# history.replaceState
--이전 주소를 없애고 바꿀 주소를 넣는다. 이전 주소가 없기 때문에 뒤로가기가 안된다.

## popstate
--pushState와 replaceState로 주소를 바꾼 후, 뒤로가기나 앞으로가기를 했을 때 발생하는 이벤트
--주의) pushState와 replaceState를 할 때는 이벤트가 발생하지 않는다. 
pushState와 replaceState를 한 후, 뒤로가기나 앞으로가기를 할 때만 발생한다.



#history.back() 
--현재 페이지의 한단계 이전 페이지로 이동

#history.go()
--이전 또는 이후 페이지 이동. 인자에 숫자를 넣어 이동한다.
----history.go(-1) //한 페이지 뒤로 가기
----history.go(1) //한 페이지 앞으로 가기 == forward
----history.go(2) //두 페이지 앞으로 가기
----history.go(-2) //두 페이지 뒤로 가기
----history.go(),history.go(0) //현재 페이지 새로고침

#history.forward() 
--다음페이지로 이동
```
