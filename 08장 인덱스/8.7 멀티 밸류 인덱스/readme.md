# 8.7 멀티 밸류 인덱스

멀티 밸류 인덱스는 하나의 레코드에 여러 개의 키 값을 가질 수 있는 형태의 인덱스다.

JSON의 배열 타입의 필드에 저장된 원소들에 대한 인덱스 요건으로 인해 최근 RDBMS에서 지원하기 시작했다.

멀티 밸류 인덱스를 활요하기 위해서는 반드시 다음 함수들을 이용해서 검색해야 옵티마이저가 인덱스를 활용한 실행 계획을 수립한다.
- MEMBER OF()
- JSON_CONTAINS()
- JSON_OVERLAPS()