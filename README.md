# Best-Worst-Fit-Memory-Allocation

This repository contains C programs implementing **Best Fit and Worst Fit memory allocation policies** for Experiment 12 of the Operating Systems lab manual.

## Programs Included

- **Best Fit (`bestfit.c`):** Allocates each application to the smallest available memory block that can accommodate it.
- **Worst Fit (`worstfit.c`):** Allocates each application to the largest available memory block that can accommodate it.
- **Comparison (`comparison.c`):** Compares the allocation results of Best Fit and Worst Fit using the same memory blocks and application sizes.

## Input Details

- Memory blocks: 50 MB, 120 MB, 80 MB
- Application sizes: 45 MB, 75 MB, 100 MB

## Requirements

- GCC compiler
- Linux terminal or Ubuntu environment

## Compilation and Execution

### 1. Best Fit

```bash
gcc bestfit.c -o bestfit
./bestfit
```

### 2. Worst Fit

```bash
gcc worstfit.c -o worstfit
./worstfit
```

### 3. Best Fit and Worst Fit Comparison

```bash
gcc comparison.c -o comparison
./comparison
```

## Expected Output

**Best Fit**
```text
45 MB -> B0
75 MB -> B2
100 MB -> B1
```

**Worst Fit**
```text
45 MB -> B1
75 MB -> B2
100 MB -> WAIT
```

**Comparison**
```text
Best Fit:
45 MB -> B0
75 MB -> B2
100 MB -> B1
Worst Fit:
45 MB -> B1
75 MB -> B2
100 MB -> WAIT
```

## Real-World Application

These programs demonstrate memory allocation for Smart TV applications, such as streaming, browser, and game apps.

## Conclusion

Best Fit selects the smallest suitable available memory block, whereas Worst Fit selects the largest suitable available memory block. The comparison demonstrates how the two policies handle the same memory requests differently.
