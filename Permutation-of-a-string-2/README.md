```
from itertools import permutations

def permute(s):
    return["".join(p) for p in permutations(s)]

s = "ABC"
print(' '.join(permute(s)))
```
