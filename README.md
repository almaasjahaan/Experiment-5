# Experiment-5
## AIM:Write a python program for Binary Search and inspect for failures. 

# ALGORITHM
Start the program.
2. Get the list from the user
3. Get the element to be searched
4. Compare the mid element with the key, if same return the index
5. If key is greater, search it in the right side, else search it in the left side.
6. If not found return -1
 7. Stop the program. 

 # PROGRAM
 ```
def binary_search(arr,target):
   low,high=0,len(arr)-1

   while low<=high:
       mid=(low+high)//2
       if arr[mid]==target:
           return mid
       elif arr[mid]<target:
           low=mid+1
       else:
           high=mid-1
   return -1

arr=[2,8,54,48,85,96]
target=int(input("Enter the number to search :"))
result=binary_search(arr,target)

if result != -1:
   print(f"{target} found at index {result}")
else:
   print(f"{target} not found in the list")
```

 # OUTPUT
 <img width="625" height="475" alt="image" src="https://github.com/user-attachments/assets/08840c97-d6ad-481b-a4aa-c860d45d2ded" />
<img width="596" height="478" alt="image" src="https://github.com/user-attachments/assets/51b22887-1854-4b9c-8bc1-ed7728eea952" />


 # RESULT
Thus the python program for Binary Search and inspect for failures is executed succesfully. 
