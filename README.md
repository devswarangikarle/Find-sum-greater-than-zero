# Find-sum-greater-than-zero
You are given an array arr of length n. In one operation, you can choose any index i and either increment arr[i] by 1 or decrement arr[i] by 1. Your goal is to find the minimum number of operations required to ensure that the sum of all elements in the array is even but not zero, i. e., the sum should be divisible by 2 and greater than 0. 

def min_operations(arr):
    even_sum = sum(arr)
    if even_sum % 2 == 1:
        return 1
    elif even_sum == 0:
        return 2
    else:
        return 0

n = int(input())
arr = list(map(int, input().split()))

print(min_operations(arr))
