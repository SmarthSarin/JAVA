# Array
An array in Java is a collection of elements of the same type, stored in a contiguous block of memory. Arrays let you store multiple values in a single variable, making it easier to manage and organize related data.

### Key Features of Arrays:
- **Fixed Size**: Once you define the size of an array, it cannot change.
- **Indexed**: Each element has an index, starting from `0` for the first element.
- **Same Data Type**: All elements in an array must be of the same type (e.g., all integers, all strings).

### Example of an Array in Java:

Let’s say you want to store the scores of five students. Instead of creating five separate variables, you can use an array.

```java
public class ArrayExample {
    public static void main(String[] args) {
        // Declare and initialize an array of integers with 5 elements
        int[] scores = {85, 90, 78, 92, 88};

        // Access and print each score using its index
        System.out.println("Score of Student 1: " + scores[0]); // 85
        System.out.println("Score of Student 2: " + scores[1]); // 90
        System.out.println("Score of Student 3: " + scores[2]); // 78
        System.out.println("Score of Student 4: " + scores[3]); // 92
        System.out.println("Score of Student 5: " + scores[4]); // 88

        // Calculate the average score
        int total = 0;
        for (int i = 0; i < scores.length; i++) {
            total += scores[i];  // Sum up all elements
        }
        double average = total / (double) scores.length;
        System.out.println("Average Score: " + average);
    }
}
```

### Explanation:
1. **Declaration and Initialization**:
   - `int[] scores = {85, 90, 78, 92, 88};` creates an array named `scores` with five elements (all integers).
   - Each element is assigned a score: 85, 90, 78, 92, and 88.

2. **Accessing Elements**:
   - `scores[0]` refers to the first element (85), `scores[1]` to the second element (90), and so on.
   - We use `System.out.println` to print each element individually.

3. **Calculating the Average**:
   - We loop through the array using `for` to calculate the total sum of scores.
   - Then, we divide the total by the length of the array (`scores.length`) to get the average score.

### Output:
```
Score of Student 1: 85
Score of Student 2: 90
Score of Student 3: 78
Score of Student 4: 92
Score of Student 5: 88
Average Score: 86.6
```

Arrays are very useful for organizing large sets of data, like lists of numbers, names, or objects.
