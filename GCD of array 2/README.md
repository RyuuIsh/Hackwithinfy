```
def gcd(a, b):
    while b:
        a, b = b , a % b
        
    return a

def find_gcd(arr):
    res = arr[0]
    for num in arr[1:]:
        res = gcd(res, num)
    return res

n = int(input())
arr = list(map(int, input().split()))
print(find_gcd(arr))
```
