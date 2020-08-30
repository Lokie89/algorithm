## 자료구조와 함께 배우는 알고리즘 입문

#### Java Collection Framework  ( List, Set, Map )

 - Collection
    - List <br>
    데이터 중복 허용, 순서 유지, 힙 영역 내에 일렬로 늘어놓아짐
        - ArrayList<br>
            인덱스를 사용하는데에 강점을 가지고 있음<br>
            빠른 조회가 강점<br>
            저장소의 용량을 늘리는 과정에서 많은 시간이 소요된다<br>
            느린 add, delete 가 단점<br>
        - Vector<br>
            ArrayList 와 동일하나 쓰레드에 안전하다.
            - Stack<br>
                후입선출
        - LinkedList<br>
            2개 크기의 배열로 앞에는 값 뒤에는 이어지는 배열의 주소값을 가지고 있음<br>
            따라서 중간 삽입, 삭제에 능함 ( 해당 부분만 고치면 되니까 )
            조회 시 index 를 사용하지 않아 처음부터 나올때까지 찾아야됨
    - Queue<br>
    선입선출
        - PriorityQueue<br>
            저장한 순서에 관계없이 우선순위가 높은 것부터 꺼낸다. ( 오름차순 등 )
        - Deque<br>
            양쪽 끝에서 추가/삭제 가능
            - ArrayDeque<br>
                스레드 안전하지 않음
            - ConcurrentLinkedDeque<br>
                스레드 안전함
            - LinkedBlockingDeque<br>
                Linked node 로 이루어짐
            - LinkedList<br>
                위의 설명
    - Set<br>
    데이터 중복 허용 X, 순서 유지 X, 인덱스가 없어서 반복자 제공
        - HashSet<br>
            객체 저장 시 저장 전 중복검사를 위해 hashCode() 와 equals() 를 호출
        - SortedSet<br>
    - Map <br>
    중복 불가 한 키와, 중복 가능한 값으로 이루어진 구조, <br>
    키 값 중복검사 시 hashCode() 와 equals() 를 호출
        - HashMap<br>
            중복을 허용하지 않고 순서를 보장하지 않는다.
