# Lab 3

## Part 1 - Bugs

The bug I am choosing is the reverse method. 

1. A failure inducing input is { 1, 2, 3 }
```
@Test
  public void testReversed() {
    int[] input2 = { 1, 2, 3 };
    assertArrayEquals(new int[] { 3, 2, 1 }, ArrayExamples.reversed(input2));
  }
```

2. An input that doesn't induce an input is { }, an empty array.
```
@Test
  public void testReversed() {
    int[] input1 = { };
    assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
  }
```

Note: I seperated the code but the original has both inputs, as seen below.
```
@Test
  public void testReversed() {
    int[] input1 = { };
    assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));

    int[] input2 = { 1, 2, 3 };
    assertArrayEquals(new int[] { 3, 2, 1 }, ArrayExamples.reversed(input2));
  }
```

3. The symptom is that it would return an array with zeros: { 0, 0, 0 }

   ![symptom](lab3_files/symptom.png)

4. Before and after code to fix it

Before:
```
  static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
```

After:
```
  static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
        newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  }
```
This fixes the issue because before it was taking the new array values which was all zeros and editing the original array to have those values. Now it takes the array values from the end of the original array and puts it at the beginning of the new array which reverses the elements.

## Part 2 - Commands


