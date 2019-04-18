# Python Interfaces

### [HackerRank](www.hackerrank.com)

> The AdvancedArithmetic interface and the method declaration for
> the abstract divisorSum(n) method are provided for you in the editor below.
> Complete the implementation of Calculator class, which implements the
> AdvancedArithmetic interface. The implementation for the divisorSum(n)
> method must return the sum of all divisors of n.

## Code

#### Since I'll need all the divisors of n, that'll be a list.

```python
[]
```

#### To grab them I can just do a for loop and add to list if n % i.

```python
[i for i in n if n % i == 0]
```

#### Sum up that list

```python
sum([i for i in n if n % i == 0]
```

## Final Code

```python
class AdvancedArithmetic(object):
    def divisorSum(n):
        raise NotImplementedError

class Calculator(AdvancedArithmetic):

    def divisorSum(self, n):
        return sum([i for i in range(1, n+1) if n % i == 0])

```

## Conclusion

Always good to keep me on my toes.
