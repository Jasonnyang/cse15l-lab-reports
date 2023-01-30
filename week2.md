## Week 2 lab report
**Part 1**

**Part 2**
<code>class EvensExample {
  static int sumEvenIndices(int[] nums) {
    int sum = 0;
    for(int i = 0; i < nums.length; i += 2) {
      sum += nums[i + 1];
    }
    return sum;
  }
}</code>
A failure-inducing input for the buggy program, as a JUnit test and any associated code (write it as a code block in Markdown)
<code>public void testSumEvensLength4() {
        int[] input1 = { 12, 13, 7, 2};
        assertEquals(EvensExample.sumEvenIndices(input1), 19);
    }</code>
An input that doesn’t induce a failure, as a JUnit test and any associated code (write it as a code block in Markdown)
<code>public void testSumEvenLength6() {
    int[] input1 = { 12, 13, 7, 8, 5, 3};
    assertEquals(EvensExample.sumEvenIndices(input1), 24);<img width="1055" alt="CleanShot 2023-01-30 at 09 27 26@2x" src="https://user-images.githubusercontent.com/36582468/215549978-16ed6143-8513-4b2a-aa43-cb63091c72cc.png">

  }</code>
The symptom, as the output of running the tests (provide it as a screenshot of running JUnit with at least the two inputs above)
The bug, as the before-and-after code change required to fix it (as two code blocks in Markdown)
  <code>class EvensExample {
  static int sumEvenIndices(int[] nums) {
    int sum = 0;
    for(int i = 0; i < nums.length; i += 2) {
      sum += nums[i + 1];
    }
    return sum;
  }
}</code>
    <code>class EvensExample {
  static int sumEvenIndices(int[] nums) {
    int sum = 0;
    for(int i = 0; i < nums.length; i += 2) {
      sum += nums[i];
    }
    return sum;
  }
}</code>
**Part 3**
