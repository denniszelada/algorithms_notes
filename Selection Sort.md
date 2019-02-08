# Selection Sort



Example sorting the most played songs

![image-20190128133909916](/Users/denniszelada/Library/Application Support/typora-user-images/image-20190128133909916.png)

In this case we are touching the list one item at a time, if we keep doing this we will end up with a sorting list

![image-20190128134031451](/Users/denniszelada/Library/Application Support/typora-user-images/image-20190128134031451.png)

![image-20190128134135983](/Users/denniszelada/Library/Application Support/typora-user-images/image-20190128134135983.png)

Example on python sort an array

```python
def findSmallest(arr):
    smallest = arr[0]
    smallest_index = 0
    for i in range(1, len(arr)):
        if arr[i] < smallest:
            smallest = arr[i]
            smallest_index = i
    return smallest_index

def selectionSort(arr):
    newArr = []
    for i in range(len(arr)):
        smallest = findSmallest(arr)
        newArr.append(arr.pop(smalest))
    return newArr

print selectionSort([5, 3, 6, 2, 10])
            
```

