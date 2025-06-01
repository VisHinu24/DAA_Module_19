# EX 1C Quick Sort
## DATE: 29-04-2025
## AIM:
To write a python program to implement quick sort using tha last element as pivot on the list of float values.

## Algorithm
1. Start by defining a function partition(arr, l, r).
2. Selects the last element of the array (arr[r]) as the pivot.
3. Define the recursive function quickSort(arr, l, r):
4. Take input for the number of elements n.
5. Read n float values into a list arr. 
6. all quickSort(arr, 0, len(arr) - 1) to sort the list.
7. Print the sorted array.

## Program:
```
/*
Program to implement implement quick sort using the last element as pivot on the list of float values.
Developed by: Vishinu H
Register Number: Reg No: 212223220124 
*/

def partition(arr,l,r):
    pivot = arr[r]
    i = l
    print("pivot: ",pivot)
    for j in range(l,r):
        if arr[j]<=pivot:
            arr[j],arr[i]=arr[i],arr[j]
            i+=1
    arr[i],arr[r]=arr[r],arr[i]
    return i
def quickSort(arr,l,r):
    if l<r:
        pivot = partition(arr,l,r)
        quickSort(arr,l,pivot-1)
        quickSort(arr,pivot+1,r)
    else:
        return
    
n = int(input())
arr = [float(input()) for i in range(n)]
quickSort(arr,0,len(arr)-1)
print(arr)
```

## Output:
![image](https://github.com/user-attachments/assets/571c1480-ad99-4b73-9789-aa60c2946d09)



## Result:
The program successfully sorts the input array using the QuickSort algorithm, arranging the elements in ascending order.
