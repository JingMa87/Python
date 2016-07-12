'''
This is the code I used for my youtube tutorial on Big O Notation (Python 3).
You can view it here: www.youtube.com/watch?v=0PPR5RWhoFI&feature=youtu.be

Big O notation is a way of writing down the time complexity of an algorithm.
Time complexity refers to how fast an algorithm works compared to the input size n.
Big O is one form of asymptotic notation. Another one is Big Theta.

Constant time: O(1)
Logarithmic time: O(log n)
Linear time: O(n)
Linearithmic time: O(n log n)
Polynomial time: O(n**2)
Exponential time: O(10**n)
'''

# O(1)
num = 10

def deductOne(num):
    num -= 1
    return num
    
print("O(1): ", "\n", deductOne(num), "\n")

# O(log n)
num = 10

def divide(num):
    while  num > 1:
        num /= 2
        print(num)
    return num

print("O(log n): ")
divide(num)
print()

# O(n)
num = 10

def addOnesToTestList(num):
    testList = []
    for i in range(0, num):
        testList.append(1)
        print(testList)
    return testList

print("O(n): ")
addOnesToTestList(num)
print()

# O(n log n)
testList = [1, 43, 31, 21, 6, 96, 48, 13, 25, 5]

def mergeSort(testList):
    if len(testList) < 2:
        return testList
    middle = int(len(testList) / 2)
    left = mergeSort(testList[:middle])
    right = mergeSort(testList[middle:])
    result = []
    print("Left: ", left)
    print("Right: ", right)
    while len(left) > 0 and len(right) > 0:
        if left[0] <= right[0]:
            result.append(left[0])
            left.pop(0)
        else:
            result.append(right[0])
            right.pop(0)
    result += left
    result += right
    print("Result: ", result)
    return result

print("O(n log n): ")
mergeSort(testList)
print()

# O(n**2)
testList = [1, 43, 31, 21, 6, 96, 48, 13, 25, 5]

def bubbleSort(testList):
    for i in range(len(testList)):
        for j in range(i+1, len(testList)):
            if testList[j] < testList[i]:
                testList[j], testList[i] = testList[i], testList[j]
            print(testList)

print("O(n**2): ")
bubbleSort(testList)

# O(10**n): trying to break a password by testing every possible combination
# (assuming numerical password of length N)

'''
Function: 10n**2 + 10n + 20
n = 1000, output: 10,010,020
'''
