# BWE objective evaluation

Mean ± std over files. Arrows: ↓ lower is better, ↑ higher is better. "baseline" is the narrowband input upsampled to 48 kHz with no BWE.

| Corpus | Mode | System | N | LSD ↓ | LSD-HF ↓ | LSD-LF ↓ | SNR ↑ |
|---|---|---|---|---|---|---|---|
| AISHELL3 | 16k→48k | baseline | 297 | 2.334 ± 0.306 | 2.809 ± 0.380 | 0.732 ± 0.070 | 29.594 ± 7.701 |
| AISHELL3 | 16k→48k | bwe | 297 | 1.030 ± 0.082 | 1.129 ± 0.096 | 0.771 ± 0.089 | 16.382 ± 2.952 |
| AISHELL3 | 8k→48k | baseline | 297 | 2.831 ± 0.345 | 3.083 ± 0.381 | 0.731 ± 0.062 | 23.068 ± 6.681 |
| AISHELL3 | 8k→48k | bwe | 297 | 1.234 ± 0.155 | 1.306 ± 0.171 | 0.726 ± 0.084 | 15.645 ± 2.627 |
| VCTK | 16k→48k | baseline | 300 | 3.333 ± 0.208 | 4.048 ± 0.254 | 0.745 ± 0.053 | 25.096 ± 5.627 |
| VCTK | 16k→48k | bwe | 300 | 1.668 ± 0.094 | 1.956 ± 0.115 | 0.806 ± 0.054 | 15.975 ± 2.142 |
| VCTK | 8k→48k | baseline | 300 | 3.740 ± 0.241 | 4.083 ± 0.264 | 0.769 ± 0.054 | 19.104 ± 4.718 |
| VCTK | 8k→48k | bwe | 300 | 1.801 ± 0.156 | 1.940 ± 0.172 | 0.753 ± 0.054 | 14.383 ± 2.420 |

## Runtime (per 70 ms frame, 200 iterations)

```
iterations: 200
8k→48k   total 382.180 ms, avg 1910.901 µs per frame
16k→48k  total 372.308 ms, avg 1861.540 µs per frame
```
