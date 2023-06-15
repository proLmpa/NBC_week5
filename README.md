# NBC_week5
* 스프링 부트로 게시판 CRUD 구현하기
  * 작성한 API 명세
  ![post api](https://github.com/proLmpa/NBC_week5/assets/52267654/2397aee6-195a-4f69-98c6-9ece4bbde703)

  * 전체 기능
    1. 전체 게시글 목록 조회
       - 어떤 request도 사용하지 않습니다.
    2. 게시글 작성
       - @RequestBody를 통해 Post 객체를 전달합니다.
    3. 선택한 게시글 조회
       - @PathVariable을 통해 url 상에 작성된 id를 전달합니다.    
    4. 선택한 게시글 수정
       - @PathVariable을 통해 url 상에 작성된 id와 @RequestBody를 통해 수정할 Post 객체를 전달합니다.
    5. 선택한 게시글 삭제
       - @PathVariable을 통해 url 상에 작성된 id와 @RequestParam을 통해 비교할 비밀번호 String을 전달합니다.

   * RESTful API 검사
     1. 각각의 자원에 접근하기 위한 고유 식별자(URI)를 부여하고 이를 통해서만 접근할 수 있게 만들었습니다.
     2. GET, POST, PUT, DELETE의 HTTP 메서드를 활용했습니다.
     3. 프로그램을 Controller, Service, Repository로 분리하여 각각 독립된 상태로 기능하게 만들었습니다.
     4. 캐시 기능 활용 여부는 조금 더 확인해보겠습니다.
