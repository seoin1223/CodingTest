# CodingTest

#### Char
<details>
  <summary>자세히</summary>

  1. Character.isUpperCase(char) : char이 대문자 여부 확인
  2. Character.isLowerCase(char) : char이 소문자 여부 확인
  3. Character.toUpperCase(char) : char의 대문자 반환
  4. Character.toLowerCase(char) : char의 소문자 반환
</details>

#### String
<details>
  <summary>자세히</summary>
  <span><b> 문자열 + int = 문자열</b></span>

  
  
  1. replaceAll(): 두 번째 매개변수로 정규 표현식과 일치하는 모든 패턴을 대체.
  2. replace(): 첫 번째 발견된 문자열만을 대체
  3. toLowerCase() : 소문자로 변환
  4. toUpperCase() : 대문자로 변환
  5. concat(String) : 문자열 합치기
  6. contains(String) : 포함하는지 여부 확인
  7. substring(int) : 해당 인덱스부터 끝까지 자르기
  8. charAt() :문자열에서 특정 위치에 있는 문자를 반환
  9. split() : 문자열을 특정 구분자를 기준으로 나누어 배열로 반환
  10. endsWith(string) : 문자열이 특정한 접미사로 끝나는지 여부 확인
  11. startsWith(string) : 문자열이 특정한 접두사로 시작하는지 여부 확인
</details>

#### StringBuilder
<details>
  <summary>자세히</summary>

  1. append(String) : 추가
  2. repeat(int) :현재 내용을 지정된 횟수만큼 반복하여 추가 -> string에서 사용 가능

</details>


#### Array
<details>
  <summary>자세히</summary>
  
  1. Arrays.copyOfRange([],int, int) : 범위를 지정해서 일부 요소만을 복사
  2. Arrays.copyOf([],int) : 처음부터 int까지를 복사
  3. System.arraycopy(Object src, int srcPos, Object dest, int destPos, int length) : 배열의 일부 또는 전체 요소를 다른 배열로 복사
       src: 복사할 배열(소스 배열)
       srcPos: 소스 배열에서 복사를 시작할 인덱스
       dest: 복사된 요소가 들어갈 대상 배열(목적지 배열)
       destPos: 대상 배열에서 복사를 시작할 인덱스
       length: 복사할 요소의 개수  

  
</details>


#### ArrayList
<details>
  <summary>자세히</summary>

  1. add() : 추가
  2. get(int) : 해당 index를 반환
  3. size() : ArrayList 크기 반환
  
</details>
