Look at the code in the cell below, but **don't run it yet**. For each `print`{.python} statement, write down what you think will be printed. Then run the cell and check whether your predictions were correct.

```py-cell
import numpy as np

a = np.array([1, 2])
b = np.array([3, 4])

print("Case 1: ", a + b)
print("Case 2: ", a / 2)
print("Case 3: ", a ** b)
print("Case 4: ", 2 - a)
print("Case 5: ", a - b * 2)
```

# Hints

> [!HIDDEN]
>
> 1. When two arrays are operated on, elementwise operations are performed.
> 2. When an array is operated on with a scalar, the operation is applied to each element of the array.
> 3. Remember the order of operations.

# Explanations

>[!HIDDEN]
>
> 1. **Case 1**: The addition of two arrays `a`{.python} and `b`{.python} will be performed elementwise. So, it will be `[1 + 3, 2 + 4]`-{.python} which results in `[4, 6]`{.python}.
> 2. **Case 2**: Dividing the array `a`{.python} by the scalar `2`{.python} will apply the division to each element of `a`{.python}. So, it will be `[1 / 2, 2 / 2]`{.python} which results in `[0.5, 1.0]`{.python}.
> 3. **Case 3**: The exponentiation of array `a`{.python} by array `b`{.python} will be performed elementwise. So, it will be `[1 ** 3, 2 ** 4]`{.python} which results in `[1, 16]`.
> 4. **Case 4**: Subtracting the array `a`{.python} from the scalar `2`{.python} will apply the subtraction to each element of `a`. So, it will be `[2 - 1, 2 - 2]`{.python} which results in `[1, 0]`.
> 5. **Case 5**: The operation `a - b * 2`{.python} will first multiply `b`{.python} by `2`{.python} (as multiplication happens before subtraction in the order of operations), resulting in `[6, 8]`, and then subtract that from `a`, resulting in `[1 - 6, 2 - 8]`{.python} which gives `[-5, -6]`.