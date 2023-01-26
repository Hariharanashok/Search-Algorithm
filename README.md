# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Linear Search:
1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.
2.	If k matches with an element in array[] , return the index.
3.	If k doesn’t match with any of elements in array[], return -1 or element not found.
## Binary Search:
1.	Set two pointers low and high at the lowest and the highest positions respectively.
2.	Find the middle element mid of the array ie. arr[(low + high)/2]
3.	If x == mid, then return mid.Else, compare the element to be searched with m.
4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.
5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.
6.	Repeat steps 2 to 5 until low meets high
## Program:
i)	#Use a linear search method to match the item in a list.
```python
#Program for linear search method to match the item in a list
#Developed by: HARIHARAN A
#RegisterNumber: 22001891
def linearSearch(array,n,k):
    # write your code for linear search
    for i in range(0,n):
        if(array[i]==k):
            return i
    return -1
    
array = eval(input())
k = eval(input()) 
n=len(array)
array.sort()
result =linearSearch(array,n,k)
if(result==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)

```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```python
#Program to find the element in a list using Binary Search(Iterative Method)..
#Developed by: HARIHARAN A
#RegisterNumber: 22001891
def binarySearchIter(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array = eval(input())
# sort the array
array.sort()
k = eval(input()) #k-item to be searched
result=binarySearchIter(array,k,0,len(array)-1)
if(result==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)

```
iii)	# Find the element in a list using Binary Search (recursive Method).
```python
#Program to find the element in a list using Binary Search (recursive Method).
#Developed by: HARIHARAN A
#RegisterNumber: 22001891
def linearSearch(array,n,k):
    for i in range(0,n):
        if(array[i]==k):
            return i
    return -1
    
array=eval(input())
k=eval(input())
n=len(array)
array.sort()
result=linearSearch(array,n,k)
if(result==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)

```
## Input 
i) #Use a linear search method to match the item in a list.
![image](https://user-images.githubusercontent.com/120353431/214833848-a1d9d0ed-3945-4afc-989b-41106e8caefa.png)
ii) #Iterative method
![image](https://user-images.githubusercontent.com/120353431/214834033-04d90f33-6abe-4828-a5a3-02c4417fbe3b.png)
iii) #Recursive method
![image](https://user-images.githubusercontent.com/120353431/214834147-e69afc80-f17f-4676-87f7-251c02bcb79f.png)

## Output
i)
![image](https://user-images.githubusercontent.com/120353431/214834306-2a91f982-034a-4f1a-a46c-c115b99fb05e.png)
ii)
![image](https://user-images.githubusercontent.com/120353431/214834367-49786daa-532a-45c8-a25b-e9e871377c26.png)
iii)
![image](https://user-images.githubusercontent.com/120353431/214834512-9ae1e134-2825-4c7d-aa47-60ba0937536c.png)


## Result
Thus the linear search and binary search algorithm is implemented using python programming.
