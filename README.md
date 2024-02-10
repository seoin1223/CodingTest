# CodingTest

## 목차
1. [용어](#용어)
2. [자료형](#1-data-types)
3. [Math](#2-math)
4. [List](#3-list)
5. [Set](#4-set)
6. [자료구조](#5-자료-구조)
7. [알고리즘](#6-알고리즘)


### 용어

1. Method Reference : 자바의 람다 표현식을 간결하게 표현하기 위한 문법
2. 문자열 + int = 문자열

<br>
<!-- 자료형 -->

### 1. Data Types

<details>
<summary> Char</summary>

1. Character.isUpperCase(char) : char이 대문자 여부 확인
2. Character.isLowerCase(char) : char이 소문자 여부 확인
3. Character.toUpperCase(char) : char의 대문자 반환
4. Character.toLowerCase(char) : char의 소문자 반환

</details>
<br>
<details>
<summary> String</summary>

1. String replaceAll(): 두 번째 매개변수로 정규 표현식과 일치하는 모든 패턴을 대체.
2. String replace(): 첫 번째 발견된 문자열만을 대체
3. String toLowerCase() : 소문자로 변환
4. String toUpperCase() : 대문자로 변환
5. String concat(String) : 문자열 합치기
6. String contains(String) : 포함하는지 여부 확인
7. String substring(int) : 해당 인덱스부터 끝까지 자르기
8. String[] split() : 문자열을 특정 구분자를 기준으로 나누어 배열로 반환
9. String trim() : 문자열의 앞과 뒤에서 공백을 제거
10. String join(CharSequence delimiter, CharSequence... elements) : 문자열을 결합할 때 사용

11. Char charAt() :문자열에서 특정 위치에 있는 문자를 반환

12. Boolean endsWith(string) : 문자열이 특정한 접미사로 끝나는지 여부 확인
13. Boolean startsWith(string) : 문자열이 특정한 접두사로 시작하는지 여부 확인

14. int indexOf(String) : 지정된 부분 문자열의 첫 번째 발생 인덱스를 반환
15. int lastIndexOf(String) : 문자열에서 주어진 문자열 또는 문자의 마지막으로 등장하는 위치의 인덱스를 반환

</details>
<br>
<details>
<summary> StringBuilder</summary>

1. append(String) : 추가
2. repeat(int) :현재 내용을 지정된 횟수만큼 반복하여 추가 -> string에서 사용 가능

</details>
<br>
<details>
<summary> Array </summary>

1. Arrays.copyOfRange([],int, int) : 범위를 지정해서 일부 요소만을 복사
2. Arrays.copyOf([],int) : 처음부터 int까지를 복사
3. System.arraycopy(Object src, int srcPos, Object dest, int destPos, int length) : 배열의 일부 또는 전체 요소를 다른 배열로 복사
    - src: 복사할 배열(소스 배열)
    - srcPos: 소스 배열에서 복사를 시작할 인덱스
    - dest: 복사된 요소가 들어갈 대상 배열(목적지 배열)
    - destPos: 대상 배열에서 복사를 시작할 인덱스
    - length: 복사할 요소의 개수
4. Boolean Arrays.equals([],[]) : 두 배열의 원소를 한번에 비교하여 boolean 값을 반환함

</details>
<br>
<!-- Math -->

### 2. Math

<details>
<summary>자세히</summary>

1. int Min(int, int) : 최소값 반환
2. int Max(int, int) : 최대값 반환
3. int ceil(int) = 항상 값을 올려서 반올림 

</details>

<br>
<!-- List -->

### 3. List

<details>
  <summary> List</summary>
  
  1. size() : List의 크기를 반환한다.
  2. indexOf(object) : List의 원소중 Object의 원소의 index를 반환
  3. List<E> subList(int from, int to) : 리스트의 일부를 추출하여 부분 리스트로 반환 (from ~ to-1)
</details>

<details>
<summary> ArrayList</summary>

1. add() : 추가
2. get(int) : 해당 index를 반환
3. size() : ArrayList 크기 반환
4. remove(int) : 지정된 인덱스에 위치한 요소를 제거 (뒤의 모든 요소를 왼쪽으로 이동)

</details>

<br>
<!-- Set -->

### 4. Set

<details>
<summary>HashSet</summary>

1. 중복 허용 x, 순서 x, null 허용
2. add(element) : 추가
3. remover(element) : 삭제
4. contains(element) : 존재 확인

</details>

<details>
<summary>LinkedHashSet</summary>

1. 중복 허용하지 않음: LinkedHashSet은 Set 인터페이스를 구현하므로 중복된 원소를 허용 x.
2. 순서 유지: 원소가 삽입된 순서대로 원소들이 유지됩니다. 따라서, LinkedHashSet을 순회하면 원소들이 삽입된 순서대로 반환.
3. 성능: 검색, 삽입, 삭제 연산은 HashSet과 유사하게 빠른 성능을 제공.
4. null 허용: LinkedHashSet도 HashSet과 마찬가지로 null 값을 허용. 

</details>

<br>

### 5. Map
<details>
   <summary>HashMap</summary>

1.  키-값(Key-Value) 쌍을 저장하는 데 사용
2. put(K key, V value): 지정된 키와 값을 매핑하여 맵에 추가합니다.
3. get(Object key): 지정된 키에 매핑된 값을 반환합니다.
4. remove(Object key): 지정된 키에 매핑된 항목을 삭제합니다.
5. containsKey(Object key): 지정된 키가 맵에 포함되어 있는지 여부를 반환합니다.
6. keySet(): 맵에 있는 모든 키를 반환합니다.
7. values(): 맵에 있는 모든 값들을 반환합니다.
8. entrySet(): 맵의 모든 키-값 쌍을 Map.Entry 객체로 반환합니다.
</details>

<br>

### 5. 자료 구조

<details> 
<summary> Stack </summary>

1. push(E item): 스택의 맨 위에 요소를 추가합니다.
2. pop(): 스택의 맨 위에서 요소를 제거하고 반환합니다.
3. peek(): 스택의 맨 위에 있는 요소를 반환하지만, 제거하지는 않습니다.
4. empty(): 스택이 비어있는지 여부를 반환합니다.
5. search(Object o): 스택에서 주어진 요소를 찾아 그 인덱스를 반환합니다.

</details>
  
 
### 6. 알고리즘

<details>
   <summary>퀵 정렬</summary>

1. 하나의 리스트를 pivot을 기준으로 두 개의 비균등한 크기로 분할하고, 분할된 부분 리스트를 정렬한 다음, 두 개의 정렬된 부분 리스트를 합하여 전체가 정렬된 리스트가 되게 하는 방법
2. 방법
   1. Divide : 입력 배열을 피벗을 기준으로 비균등하게 2개의 부분 배열로 분할
   2. Conquer : 부분 배열을 정렬 (부분 배열의 크기가 충분히 작지 않으면 순환 호출을 이용하여 다시 분할 정복 방법 적용)
   3. Combine : 정렬된 부분 배열들을 하나의 배열에 합병한다.
   
</details>


  
