# Reflection

## 1. When did the baseline become sluggish?
The baseline became noticeable at n = 2,500 (about 0.23 s) and clearly slow
at n = 5,000 (0.87 s) and n = 10,000 (3.74 s). Kadane's stayed around a
millisecond even at n = 10,000.

## 2. Baseline estimate for n = 1,000,000
The baseline is O(N²): doubling n roughly quadruples the time (0.87 s -> 3.74 s
from n = 5,000 to 10,000). Going from n = 10,000 to n = 1,000,000 is a 100x
increase, so the time grows by about 100² = 10,000x.

3.743 s x 10,000 ≈ 37,433 s ≈ 10.4 hours.

## 3. Kadane's estimate for n = 1,000,000
Kadane's is O(N): doubling n roughly doubles the time (0.000509 s -> 0.001054 s).
A 100x increase in n means about 100x the time.

0.001054 s x 100 ≈ 0.105 s.