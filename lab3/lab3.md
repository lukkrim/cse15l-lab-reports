## Part 1
Bug Chosen
1. Failer-inducing input<br>
```
@Test 
public void testReverseInPlace() {
  int[] input1 = {1,2,3};
  ArrayExamples.reverseInPlace(input1);
  assertArrayEquals(new int[]{3,2,1}, input1);
}
```
