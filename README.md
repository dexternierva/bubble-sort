# Bubble Sort
Accepts an array and returns a sorted version of the array

## Pseudocode
1. Create a function that accepts an array of numbers as a parameter
2. Create a loop that walks through the array
3. Create an inner loop that handles the comparison of each numbers to its neighbor on the right
4. Inside the inner loop, if a number is greater than the value of its neighbor to the right swap the values

### JavaScript Code
```javascript
function bubbleSort (array) {
    for (let i = array.length; i > 0; i--) {
        for (let j = 0; j < i; j++) {
            if (array[j] > array[j + 1] ) {
                let temp = array[j];
                array[j] = array[j + 1];
                array[j + 1] = temp;
            }
        }
    }

    return array;
}
```
