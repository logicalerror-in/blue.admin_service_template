# blue.admin_service_template

Admin domain service 생성을 위한 기준 template 저장소입니다.

## 역할

- admin service 기본 구조 제공
- Resource Server 기준 제공
- DB migration 기준 제공
- outbox event 발행 기준 제공 후보

## 기술 후보

- Java / Spring Boot 우선
- Python / FastAPI 허용
- 필요 시 Kotlin, Go 등 검토

## 책임 경계

각 service는 자기 도메인 비즈니스 로직을 소유합니다.
각 service는 fine-grained authorization을 유지합니다.
Gateway의 공통 검증만 신뢰하고 business permission은 직접 판단합니다.

## 관련 예시

- admin-etf
- admin-collector
- admin-analysis
