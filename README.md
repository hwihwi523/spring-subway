# 지하철 노선도

## 요구사항

### 구조
* 지하철 역
  * id
  * name
* 지하철 구간
  * id
  * 상행 역 id
  * 하행 역 id
  * 노선 id
  * distance
* 지하철 노선
  * id
  * name
  * color

### 구간 등록 기능
* 지하철 노선에 구간을 등록할 수 있다.
* 새로운 구간의 상행역은 노선에 등록되어 있는 하행 종점역이어야 한다.
* 새로운 구간의 하행역은 노선에 등록되어 있지 않아야 한다.
* 위 조건에 부합하지 않는 경우에는 에러 처리한다. 400?
  * 새로운 구간의 상행역이 하행 종점역과 다를 경우
  * 새로운 구간의 하행역이 노선에 등록되어 있을 경우

### 구간 제거 기능
* 지하철 노선에서 구간을 제거할 수 있다.
* 하행 종점역만 제거할 수 있다.
* 구간이 1개인 경우 삭제할 수 없다.
* 위 조건에 부합하지 않는 경우에는 에러 처리한다. 400?
