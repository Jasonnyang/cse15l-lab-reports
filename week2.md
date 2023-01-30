## Week 2 lab report
**Part 1**

**Part 2** <br>
```java
class EvensExample {
  static int sumEvenIndices(int[] nums) {
    int sum = 0;
    for(int i = 0; i < nums.length; i += 2) {
      sum += nums[i + 1];
    }
    return sum;
  }
}
```
A failure-inducing input for the buggy program
```java
public void testSumEvensLength4() {
    int[] input1 = { 12, 13, 7, 2};
    assertEquals(EvensExample.sumEvenIndices(input1), 19);
}
```
An input that doesn’t induce a failure
```java
public void testSumEvenLength6() {
    int[] input1 = { 12, 13, 7, 8, 5, 3};
    assertEquals(EvensExample.sumEvenIndices(input1), 24);
}
```
The symptom, as the output of running the tests<br>
The program is summing all of the odd indexes instead of the even indexes
<img width="1055" alt="CleanShot 2023-01-30 at 09 27 26@2x" src="https://user-images.githubusercontent.com/36582468/215549978-16ed6143-8513-4b2a-aa43-cb63091c72cc.png">
The bug, as the before-and-after code change required to fix it
```java
class EvensExample {
  static int sumEvenIndices(int[] nums) {
    int sum = 0;
    for(int i = 0; i < nums.length; i += 2) {
      sum += nums[i + 1];
    }
    return sum;
  }
}
```
```java
class EvensExample {
  static int sumEvenIndices(int[] nums) {
    int sum = 0;
    for(int i = 0; i < nums.length; i += 2) {
      sum += nums[i];
    }
    return sum;
  }
}
```
This fix addresses the issue because originally we were adding 1 to all of the indexes being summed so index 1, 3, 5, etc. were being summed instead of 0, 2, 4, etc. By removing the [i+1] and replacing it with [i] it allows the even indexes to be summed instead of the odd ones. <br>
**Part 3**

