## Part 1
I chose the bug in the `reverseInPlace` method in the `ArrayExamples` class.
### Failure-inducing input in the new method `testReverseInPlaceTwo` in the `ArraryTests` class

```
@Test
public void testReverseInPlaceTwo() {
    int[] input1 = {1, 2, 3, 4, 5};
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{5, 4, 3, 2, 1}, input1);
	}
```

### An input in the new method `testReverseInPlaceThree` that doesn't induce a failure in the `ArrayTests` class.

```
@Test 
	public void testReverseInPlaceThree() {
    int[] input1 = { 4 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 4 }, input1);
	}
```
### When it was run with a JUnit test with the two inputs above, the following result was generated
![image](JUnitFail.png)

### The code for `reverseInPlace` method before fix
```
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
```

### The code for `reverseInplace` method after fix	
```
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length / 2; i++) {
        int temp = arr[i];
        arr[i] = arr[arr.length - i - 1];
        arr[arr.length - i - 1] = temp;
    }
}
```

## Part 2
