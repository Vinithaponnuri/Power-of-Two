# Power-of-Two
class Solution:
    def isPowerOfTwo(self, n: int) -> bool:
        if n==1:
            return True
        if n<1:
            return False
        return self.isPowerOfTwo(n//2) if n%2==0 else False
                             
                             OR
                             
class Solution:
    def isPowerOfTwo(self, n):
        if n==0:
            return False
        while(n!=1):
            if n%2!=0:
                return False
            n=n//2
        return True                             
