# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```
''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: PERARASU M
RegisterNumber: 212222100033
'''
def selection_sort(nums):
    for i in range(len(nums)):
        low=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[low]:
                low=j
        nums[i],nums[low]=nums[low],nums[i]
    print(nums)
  
    
list_of_nums = eval(input())
selection_sort(list_of_nums)




```
ii)	#Insertion Sort
```

''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: PERARASU M
RegisterNumber: 212222100033
'''
def insertion_sort(num):
    for i in range(1,len(num)):
        insert=num[i]
        j=i-1
        while j>=0 and num[j]>insert:
            num[j+1]=num[j]
            j-=1
        num[j+1]=insert
    print(num)
    
    
    
    
list_of_nums = eval(input())
insertion_sort(list_of_nums)




```

## Output:
SELECTION SORTl:
![Screenshot 2023-06-03 170613](https://github.com/PERARASU10/Sorting-Algorithm/assets/118348589/a11e3810-b916-41ea-9734-6ba7c175a5e1)

INSERTION SORT:
![Screenshot 2023-06-03 170648](https://github.com/PERARASU10/Sorting-Algorithm/assets/118348589/e09513b2-0628-4a4d-9ff5-64d2456c525a)


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
