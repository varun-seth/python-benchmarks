Python 3.11 is about 45-50% faster for simple functions.

|    | version   |   count |     mean |   latest_improvement |
|---:|:----------|--------:|---------:|---------------------:|
|  0 | 3.7.15    |     100 | 0.33771  |             0.46293  |
|  1 | 3.8.15    |     100 | 0.350593 |             0.482665 |
|  2 | 3.9.15    |     100 | 0.353922 |             0.487531 |
|  3 | 3.10.8    |     100 | 0.347675 |             0.478323 |
|  4 | 3.11.0    |     100 | 0.181374 |             0        |

Here `mean` is the average duration (in seconds) for calculating fibonacci sequence (30th value).

Here's the fibonacci function.

```py
def fibonacci(n):
    if n == 0:
        return 0
    if n == 1:
        return 1
    return fibonacci(n-1) + fibonacci(n-2)

```

n was 30 (constant), and 100 iterations were run for each version of python
