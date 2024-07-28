class Solution:
    def fib(self, n: int) -> int:
        f0 = 0
        f1 = 1
        fn = 1

        if n == 0 :
            return f0

        for i in range(n-1):
            fn = f1 +f0
            f0 = f1
            f1 = fn
        
        return fn
