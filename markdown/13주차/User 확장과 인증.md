<h1>User 확장과 인증</h1>

* 여러 명의 사용자가 동시에 서버에 요청을 보낼 경우, 서버는 user모델을 사용해 사용자 식별

* 장고에서는 user 모델(테이블) 지원

  * 이 user를 다른 user로 대체하려면 대체할 user를 상속시키면 됨

    

* 장고에서는 auth(authentication : 인증) 지원

  1. 클라이언트가 서버에 회원가입 요청(form 작성)

  2. 서버가 이를 DB에 저장

  3. 클라이언트가 나중에 이 정보로 로그인 요청

  4. 서버가 DB를 확인해 정보가 맞을 경우 클라이언트에 token 제공(장고에서 자동 처리)