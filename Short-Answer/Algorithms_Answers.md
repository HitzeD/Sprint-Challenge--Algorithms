#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) O(n)


b) O(n^2)


c) O(n)

## Exercise II

- using merge sort kind of approach by splitting `n` in half
- on each half, check to see which half the egg breaks on
- continue breaking the number in half to locate which floor `f` is the breaking point

def egg_break(n, range=None):
    top = range(n, n - n/2)
    bottom = range(0, n - n/2)
    n = n - n/2

    if range == 1:
        return n
    else:
        if break in n:
            return egg_break(n, bottom)
        elif not break:
            return egg_break(n, top)

O(n log n)

