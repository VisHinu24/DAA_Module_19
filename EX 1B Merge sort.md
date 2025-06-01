# EX 1B Merge Sort
## DATE: 29-04-2025
## AIM:
To write a python program to sort the first half of the list using merge sort.

## Algorithm
1. Start the program.
2. Accept n, the number of elements in the list, and take input for all elements into the list inp_arr.
3. Split the list into two halves:
4. Call the recursive merge_sort() function to sort only the first_half: 
5. Replace the original first half in inp_arr with the sorted first_half.
6. End the program.

## Program:
```
/*
Program to implement Merge Sort
Developed by: Vishinu H
Register Number: 212223220124
*/
def merge_sort(inp_arr):
    if len(inp_arr) > 1:
        mid = len(inp_arr) // 2
        left = inp_arr[:mid]
        right = inp_arr[mid:]

        merge_sort(left)
        merge_sort(right)

        i = j = k = 0

        while i < len(left) and j < len(right):
            if left[i] < right[j]:
                inp_arr[k] = left[i]
                i += 1
            else:
                inp_arr[k] = right[j]
                j += 1
            k += 1

        while i < len(left):
            inp_arr[k] = left[i]
            i += 1
            k += 1

        while j < len(right):
            inp_arr[k] = right[j]
            j += 1
            k += 1

inp_arr = []     
n = int(input())
for i in range(n):
    inp_arr.append(int(input()))

print("Given array is")
print(*inp_arr)

merge_sort(inp_arr)

print("Sorted array is")
print(*inp_arr)

```

## Output:
![image](https://github.com/user-attachments/assets/52d482c9-8ea6-48fa-bdf6-da7cd395dc71)


## Result:
The program successfully sorts the first half of the given array using merge sort. where only the first half is sorted, and the second half remains unchanged.
