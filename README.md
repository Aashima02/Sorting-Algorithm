# Selection sort and Insertion sort
## AIM:
To write a program to perform selection sort and insertion sort using python programming.

## EQUIPMENT'S REQUIRED:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner

## ALGORITHM:
### Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.

### Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.

## PROGRAM:

### Selection Sort:
```
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: Aashima Nazreen Sayeed S
RegisterNumber: 21500368

def selection_sort(nums):
    for i in range(len(nums)):
        low_index=i
        for j in range(i+1,len(nums)):
            if (nums[j]<nums[low_index]):
                low_index=j
        nums[i],nums[low_index]=nums[low_index],nums[i]
    return nums
list_of_nums = eval(input())
value=selection_sort(list_of_nums)
print(value)
```

### Insertion Sort:
```
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: Aashima Nazreen Sayeed S
RegisterNumber: 21500368

def insertion_sort(nums):
    for i in range(1,len(nums)):
        item = nums[i]
        j = i-1
        while j>=0 and nums[j]>item:
            nums[j+1] = nums[j]
            j-=1
        nums[j+1] = item
    return nums
list_of_nums = eval(input())
value = insertion_sort(list_of_nums)
print(value)
```

## OUTPUT:
### Selection Sort:
![output1](https://user-images.githubusercontent.com/93427086/148724903-3989ea25-042c-4eff-aa9f-d260378cd1a0.png)

### Insertion Sort:
![output2](https://user-images.githubusercontent.com/93427086/148724921-eb6e2169-0559-4c67-ac58-cefbc98b1780.png)


## RESULT:
Thus the program is written to perform selection sort and insertion sort using python programming.
