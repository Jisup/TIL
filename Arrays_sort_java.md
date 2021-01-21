<h1>Custom 2DArrays Sort</h1>

---
<h3>Example</h3>

학생의 점수와 번호를 정렬하고 싶을 때,

```java
class student {
    double score;
    int index;
}
> student st = new student[MAX];
```

일때 score기준 object정렬

```java
Arrays.sort(st, new __Comparator<student>()__ {
    public int compare(student o1, student o2) {
        return __o1.score > o2.score? 1 : 0__;
    }
});
```

JAVA compare의 default return 타입은 boolean

```java
Arrays.sort(st, new __Comparator<student>()__ {
    public int compare(student o1, student o2) {
        return o1.score > o2.score ? 1 : (o1.score == o2.score ? (o1.index > o2.index ? 1 : 0) : 0);
    }
});  
```

score정렬 이후 index정렬 할시에 작성!
큰 문법은 C/C++과 큰차이 없다 생각된다.

---
