# Redshift Benchmark 튜토리얼

- Redshift 클러스터를 만들때 multiple node(2개 이상)를 사용하지 않으면 성능 향상을 기대하기 어렵다.
- d1.large 노드 4개로 테스트를 진행해보자. SortKey와 DistributionKey를 사용해 성능이 얼마나 달라지는지 보자.

## 1. Redshift 클러스터 만들기
## 2. 데이터 로드하기
## 3. 


```
select count(*) from LINEORDER;
select count(*) from PART;
select count(*) from  CUSTOMER;
select count(*) from  SUPPLIER;
select count(*) from  DWDATE;
```
