# WarpFrac — High-Performance Fraction Arithmetic

The world's fastest exact math library, period. It runs on almost any modern computer and has an optional GPU accelerator for unprecedented supercomputing speeds.

# INT8→INT32 Exact GEMM — Public Benchmark

**Device:** NVIDIA A100-SXM4-40GB  
**Arithmetic:** INT8×INT8 accumulate to INT32 (ROW), exact dyadic: `C_real = C_int32 * 2^-(fracA+fracB)` with `fracA=4, fracB=4`.

---

## Headline (macro arena)

- **Throughput:** **299.76 T-ops/s**  
- **Config:** M=N=K=5120, streams=32, nodes=64, tileK=1280 (panels=4), epochs=2  
- **Algo:** cuBLASLt (algo_index=0, ws=1 GB)  
- **Exactness:** micro validator **PASS** vs CPU int32; **GMP** sampled dot-products **match**, dyadic rationals printed.





