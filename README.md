https://ebook-product.kyobobook.co.kr/dig/epd/ebook/E000003336666 

# RESTAPI
- 클라이언트/서버 (Client/Server)
- 균일한 인터페이스 (Uniform Interface)
- 계층 시스템 (Layered System)
- 캐시 (Cache)
- 상태 없음 (Stateless)
- 주문형 코드 (Code-on-demand)

# 1. 클라이언트/서버
- 관심사 분리
- 일관된 인터페이스 기반
- 클라이언트/서버는 독립적 구현, 배포

# 2. 균일한 인터페이스
- 매체간 인터페이스는 각 인터페이스의 일관성에 기반
- 네 가지 인터페이스 제약
    - 리소스 식별
    - 표현을 통한 리소스 처리
    - 자기-서술적 메시지(Self-descriptive messages)
    - 애플리케이션 상태 엔진으로서의 하이퍼미디어(HATEOAS)

## 2.1. 리소스 식별
리소스는 웹 상에서 서로 구별되는 개념

## 2.2. 표현을 통한 리소스 처리
- 클라이언트는 리소스 표현 처리
- 같은 리소스라도 다른 클라이언트에서 다른 방식으로 표현될 수 있다.
    - 웹 브라우저 HTML 표현
    - 특정 프로그램 JSON 표현
- 표현은 리소스와 상호작용하는 방법, 리소스 그 자체가 아니다.

## 2.3. 자기-서술적 메시지
- **리소스 요청 상태**는 클라이언트의 **요청 메시지**로 표현
- **리소스의 현재 상태**는 그 요청에 응답하는 서버의 **응답 메시지**로 표현되어, 클라이언트에 전달
- 자기-서술적 메시지는 메타데이터를 포함
    - 리소스의 상태
    - 표현 형식과 크기
    - 메시지 자신에 대한 추가 정보
- HTTP 메시지는 일정한 형태로 여러 종류의 메타데이터 정보를 넣을 수 있는 헤더를 제공한다.

## 2.4. 애플리케이션 상태 엔진으로서의 하이퍼미디어
- 리소스의 상태 표현은 관련 리소스의 링크를 포함

# 3. 계층 시스템
- 프락시, 게이트웨이
    - 보안 강화
    - 캐싱
    - 부하 분산

# 4. 캐시
- 지연 감소
- 이용 가능성, 안정성 향상
- 웹 서버의 부하 제어
- 비용 감소

# 5. 상태 없음
- 웹 서버가 클라이언트의 상태를 관리할 필요가 없다는 의미다.
- 웹 서버는 웹 애플리케이션과의 복잡한 커뮤니케이션을 위해 필요한 상태 관리를 클라이언트에 맡김으로써 더 많은 클라이언트에 서비스 할 수 있다. 
- 이러한 트레이드오프는 웹 구조적인 스타일의 확장성에 이바지하는 주요 요소다.

# 6. 주문형 코드
- 스크립트, 플러그인의 클라이언트 실행
- 자바 애플릿, 자바스크립트


# 응답 상태 범주
1xx: 정보
2xx: 성공
3xx: 재전송
4xx: 클라이언트 오류
5xx: 서버 오류

---

- URI 경로 세그먼트는 언제 복수로 써야 하는가?
- 리소스의 상태를 업데이트하려면, 어떤 메서드를 사용해야 하는가?
- CRUD가 아닌 연산을 어떻게 URL에 매핑하는가?
- 특정한 시나리오에 가장 적합한 HTTP 응답은 무엇인가?
- 리소스 상태 표현의 버전은 어떻게 관리할 수 있는가?
- JSON에 포함된 하이퍼링크는 어떻게 구조화하는가?

