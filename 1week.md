<img width="230" alt="image" src="https://github.com/user-attachments/assets/e3af2730-6f36-4643-90e7-7750a19106aa" />



SELECT

Col1 As new_name,

Col2,

Col3

FROM Dataset. Table : 어떤 테이블에서 데이터를 확인 할건지

WHERE

Col1 = 1



'*' 모든 컬럼을 출력하겠다
  
SELECT

 * EXCEPT (제외할 컬럼)

   
이런 형태도 가능


모아서 계산하기(=그룹화)해서 계산하다


GROUP BY : 같은 값끼리 모아서 그룹화한다

특정 컬럼을 기준으로 모으면서 다른 컬럼에서 집계 가능 (합, 평균, max, min 등)


DISTINCT 

여러 값 중에 Unique한 것만 보고 싶은 경우




