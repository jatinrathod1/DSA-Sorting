# Sorting Algorithms in C++

This project contains implementations of three basic sorting algorithms: Bubble Sort, Selection Sort, and Insertion Sort in C++.

## Introduction

Sorting algorithms are fundamental to computer science and are widely used in various applications. This project demonstrates three common sorting algorithms: Bubble Sort, Selection Sort, and Insertion Sort. Each algorithm has its own approach to sorting an array of integers.

## Algorithms

### 1. Bubble Sort

Bubble Sort repeatedly steps through the list, compares adjacent elements and swaps them if they are in the wrong order. The pass through the list is repeated until the list is sorted.

### 2. Selection Sort

Selection Sort divides the input list into two parts: a sorted sublist of items which is built up from left to right at the front (left) of the list and a sublist of the remaining unsorted items. The algorithm proceeds by finding the smallest (or largest, depending on sorting order) element from the unsorted sublist, swapping it with the leftmost unsorted element (putting it in sorted order), and moving the sublist boundaries one element to the right.

### 3. Insertion Sort

Insertion Sort builds the final sorted array (or list) one item at a time. It is much less efficient on large lists than more advanced algorithms such as quicksort, heapsort, or merge sort.

## Code Explanation

### Main Function

The `main` function initializes an array of integers and calls the sorting functions:

```cpp
int main() {
    int a[] = {3, 5, 2, 7, 1};
    int n = sizeof(a) / sizeof(a[0]);

    cout << "Bubble Sort: ";
    bubbleSort(a, n);

    int b[] = {3, 5, 2, 7, 1}; // Re-initialize array for next sort
    cout << "Selection Sort: ";
    selectionSort(b, n);

    int c[] = {3, 5, 2, 7, 1}; // Re-initialize array for next sort
    cout << "Insertion Sort: ";
    insertionSort(c, n);

    return 0;
}
