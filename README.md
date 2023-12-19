# Insertion-Sort-And-Searching-Checkpoint

INSERTION SORTING AND SEARCHING CHECKPOINT
PROBLEM STATEMENT
To sort the elements of an array, and place them in their correct positions.
PSEUDOCODE
1.	Input: Input an array of elements to be sorted
2.	Iterative insertion: iterate over each element in the array from index 1 to the end such that; for each element at index ‘i’, consider the elements in the array from index 0 to i – 1 as the sorted sequence.
3.	Insertion process: 
 a.	Compare the element at index ‘i’ with the elements in the sorted sequence.
 b.	Shift elements in the sorted sequence to the right until the correct position for the element at index ‘i’ is found.
 c.	Insert the element at index ‘i’ into the correct position in the sorted sequence.
4.	Output: The array is now sorted.

 procedure insertionSort(arr):
      n = length(arr)

    for i from 1 to n-1:
        key = arr[i]
        j = i - 1

        // Move elements of arr[0..i-1] that are greater than key
        // to one position ahead of their current position
        while j >= 0 and arr[j] > key:
            arr[j + 1] = arr[j]
            j = j - 1

        // Insert the key into its correct position
        arr[j + 1] = key
