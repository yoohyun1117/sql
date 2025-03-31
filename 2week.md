# 2주차

### WHERE 절
- 조건을 연결할 때는 `AND`, `OR` 사용
  - 복잡한 조건에서는 `OR` 문에 괄호를 사용하여 가독성과 정확성 확보
- `WHERE`에서는 집계 함수(`COUNT`, `SUM` 등)를 직접 사용할 수 없음
  - `GROUP BY` 또는 `HAVING`에서 사용해야 함
- `WHERE` vs `HAVING`
  - `WHERE`: 원본 테이블에서 조건 필터링
  - `HAVING`: 그룹화 이후 조건 필터링

### GROUP BY
- `GROUP BY`에 사용하는 컬럼은 `SELECT`에도 반드시 포함되어야 함
- `GROUP BY 1, 2`처럼 `SELECT` 문 기준으로 열 번호를 사용할 수 있음

### COUNT 함수
- DAU(Daily Active Users)는 `COUNT(DISTINCT user_id) AS dau`로 구함
- `COUNT(DISTINCT ...)`를 사용해서 중복 여부를 비교해볼 수 있음
- `COUNTIF(조건)`을 사용하면 조건에 해당하는 데이터 개수를 셀 수 있음

### 기타 사항
- `NULL`은 `0`이나 `""`(빈 문자열)과 다름


## GROUP BY ALL

- `GROUP BY ALL`을 사용하면 `SELECT`에 포함된 모든 컬럼을 자동으로 그룹화할 수 있음
- 컬럼이 많을 때 유용하게 사용 가능

## SQL 쿼리 작성 흐름

1. 지표 고민: 문제 정의 후 필요한 데이터 추출
2. 지표 구체화: 분자/분모 명확히 작성, 컬럼명·테이블·조건을 구체화
3. 지표 탐색: 유사 문제 해결 사례나 기존 쿼리 참고
4. 쿼리 작성
   - 데이터가 어느 테이블에 있는지 확인
