# Fibanacci-Series

### Normal Recursion Method:

      def fib(n):
        if(n<=2):
            return 1
        return fib(n-1)+fib(n-2)

      m=fib(50)
      print(m)

### Using a Dictionary

            def fib(n,memo={}):
                if n in memo:
                    return memo[n]
                if(n<=2):
                    return 1
                memo[n]=fib(n-1,memo)+fib(n-2,memo)
                return memo[n]
            m=fib(50)
            print(m) 
