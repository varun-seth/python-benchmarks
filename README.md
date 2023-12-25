Python 3.11 is about 45-50% faster for simple functions than previous versions of python.

|    | version   |   count |     mean |   latest_improvement |
|---:|:----------|--------:|:---------|:---------------------|
|  0 | 3.7.17    |     100 | 0.425265 |            0.551687  |
|  1 | 3.8.18    |     100 | 0.399123 |            0.522323  |
|  2 | 3.9.18    |     100 | 0.406086 |            0.530513  |
|  3 | 3.10.13   |     100 | 0.390124 |            0.511304  |
|  4 | 3.11.7    |     100 | 0.188615 |           -0.0107982 |
|  5 | 3.12.1    |     100 | 0.190652 |            0         |

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
