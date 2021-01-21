# Readme.md

---
<h3>call by reference</h3>

```java
//C++이랑 다른점
public class Example {
	public static void main(String[] args) {
		int arr[] = {1,2,3};
		fucn(arr);
		System.out.println(Arrays.toString(arr));
	}
	static void fucn(int[] arr) {
		arr[0]*=2;
		arr[1]*=2;
		arr[2]*=2;
	}
}
```
