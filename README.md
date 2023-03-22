# DataStructure

## Array

- 데이터의 논리적 순서와 물리적 순서가 동일
- 원칙적으로 데이터에 대한 접근 시간은 동일
- 데이터의 삽입과 삭제시 추가적인 자료의 이동이 발생

## Linked List

- 각 데이터 시퀀스가 순서를 가지고 연결된 순차적 구조
- 동적인 데이터 추가/삭제에 유리하다.
- 각 요소는 Node
- 각 Node에는 key와 다음 노드를 가리키는 포인터인 next가 포함
- 첫 번째 요소는 Head
- 마지막 요소는 Tail

## Stack

- 순서가 보존되는 선형 데이터 구조
- 가장 마지막 요소부터 처리하는 LIFO

## Que

- 가장 먼저 입력된 요소를 처리하는 FIFO
- 멀티 스레딩에서 스레드를 관리

## Heap

- Binary Tree
- 최소힙:부모의 키 값이 자식의 키 값보다 작거나 같다
- - 루트 노드의 키 값이 트리의 최솟값
- 최대힙:부모의 키 값이 자식의 키 값보다 크거나 같다.
- - 루트 노드의 키 값이 트리의 최솟값

## Hash table

- 해시함수를 사용하여 변환한 값을 색인으로 삼아 키와 데이터를 저장하는 자료구조

## Tree

- 그래프가 계층적 구조를 가진 형태
- 최상위 노드를 가지고 있다.
- 상위 노드를 parent node ,하위 노드를 child node라 한다.
- Binary Trees
- Binary Search Tree
- Heap

## Graph

- nodes/vertices사이에 edge가 있는 collection
- directed그래프는 일방통행
- undirected그래프는 양방향
- 소셜미디어 네트워크를 나타내는데사용

### 알고리즘

- 입출력,명확성,유한성,유효성
- 모든 명령은 컴퓨터에 수행,효율적,단순명료,일정한 단계후 반드시 종료

## 알고리즘 설계기법

- 분할정복
- 동적프로그래밍
- 욕심쟁이,탐욕

메모리양 -> 공간복잡도
수행시간 -> 시간복잡도

시간복잡도 알고리즘 단계의 단위 연산의 수행 횟수의 합

- 입력크기,입력 데이터의 상태가 증가하면 수행시간도 증가
- Bigo
- 빅오메가
- 빅세타
- 재귀함수

## 1)분할정복

- 순한적으로 문제를 푸는 하향식 접근방법
- 주어진 문제의 입력을 나눌수 없을떄까지 두개이상의 작은 문제들로 순한분할하고
  분할된 작은 문제들을 각각 해결 후 이들의 해를 결합하여 문제의 해를 구하는 방법
- 분할,정복,결합
- 이진탐색
- 합병정렬
- 퀵정렬
- 선택문제

## 분할정복)합병정렬

- 입력크기가 n인 문제를 크기가 n/2인 두개의 작은 문제를 분할하고 분할된 두 작은 문제에 대해서 순한적으로 호출하여 주어진 문제를 해걀하는 것으
- 합병정렬에서 크기가 각각 n인 정렬된 두 부분 배열을 하나의 정렬배열로 합병할떄 걸리는 시간
- 합병함수 Merge- 정렬된 두 부분배열을 하나의 정렬배열로 만드는 함수
- O(n)
- tn= 2t(n/2)+0n
- 같은크기의 두 부분배열을 분할하고 순한 호출하여 정렬
- 정렬된 두 부분배열을 합쳐서 하나의 정렬배열을만듬
- 성능 t(n)= 2T(n/2)+0(n),T(1)= 0(1)->o(nlogn)
- 입력크기 n만큼의 추가적인 저장 장소필요

## 분할정복)선택문제

- n개의 원소가 순서로 저장된 배열 a[0..n-1]에서 i번쨰로 작은 원ㅇ소를 찾는 문제
- /5 나머지 버리고 그룹의 개수 (중간값들의 중간값 이용)
- 최소값찾기 적어도 (n-1)번 비교 o(n)
- 최솟값과 최대값 모두찾기 3n/2 -2번비교 O(n)
- 퀵정렬의 partition이용 최악 O(n2),평균 O(n)
- 중간값들의 중간값 이용 최악 O(n) 평균 O(n)

## 동적프로그램

- 피보나치 수열문제
- 연쇄 행렬곱셈문제
- 스트링 편집 거리문제
- 모든 정점간의 최단경로
- 저울문제

## 동적프로그래밍)피보나치수열

## 욕심쟁이

- 동전거스름돈 문제
- 배낭문제
- 최소신장트리
- 최단경로
- 작업스케줄링 문제
- 작업 선택문제
- 허프만 코딩
