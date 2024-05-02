## Part 1
**Bug Chosen: testReverseInPlace method in the ArrayExamples.java**
1. **Failer-inducing input**
```
@Test 
public void testReverseInPlace() {
  int[] input1 = {1,2,3};
  ArrayExamples.reverseInPlace(input1);
  assertArrayEquals(new int[]{3,2,1}, input1);
}
```

2. **An input that doesn't indue a failure**
```
@Test 
public void testReverseInPlace() {
  int[] input1 = {3};
  ArrayExamples.reverseInPlace(input1);
  assertArrayEquals(new int[]{3}, input1);
}
```

3. **Symptoms**<br>
Passed Test<br>
<img src = "passed.png"><br><br>
Failed Test<br>
<img src = "failed.png"><br><br>

4. **Code**<br>
Code Before
```
static void reverseInPlace(int[] arr) {
  for(int i = 0; i < arr.length; i += 1) {
    arr[i] = arr[arr.length - i - 1];
  }
}
```

Code After
```
static void reverseInPlace(int[] arr) {
  int[] temp = new int[arr.length];
  for(int i = 0; i < arr.length; i++){
    temp[i] = arr[i];
  }
  
  for(int i = 0; i < arr.length; i += 1) {
    arr[i] = temp[arr.length - i - 1];
  }
}
```

5. **Explanation of my solution**<br>
The original code does not work because it sets `arr[i]` to `arr[arr.length-i-1]`. However the second half elements of the array value will remin unchanged after the loop ends because the first half elements of the array are no longer their original value.<br>
For example, here is a demonstration on how the wrong method works<br>
`[1,2,3,4]`<br>
`[4,2,3,4]`: `arr[0] = arr[3]`<br>
`[4,3,3,4]`: `arr[1] = arr[2]`<br>
`[4,3,3,4]`: `arr[2] = arr[1]`<br>
`[4,3,3,4]`: `arr[3] = arr[0]`<br><br>
For the fixed function, I first create a temperaory array that copies all the elements of the original array over. Therefore, when we perform the setting line of code, we will use `arr[i] = temp[arr.length - i - 1]` instead of `arr[i] = arr[arr.length - i - 1]` so that we will use the original value of each element from the temp array.<br>
For example, here is a demonstration on how the correct method works<br>
`[1,2,3,4]`<br>

## Part 2
`[4,2,3,4]`: `arr[0] = temp[3]`<br>
`[4,3,3,4]`: `arr[1] = temp[2]`<br>
`[4,3,2,4]`: `arr[2] = temp[1]`<br>
`[4,3,2,1]`: `arr[3] = temp[0]`<br><br>

