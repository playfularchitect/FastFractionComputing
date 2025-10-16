# WarpFrac — High-Performance Fraction Arithmetic

The world's fastest exact math library, period. It runs on almost any modern computer and has an optional GPU accelerator for unprecedented supercomputing speeds.
This is a **binary only evaluation release** for testing and validation. 
Commercial licensing available for production use.

---

## Performance Benchmarks

The following benchmarks were recorded using the provided Google Colab notebooks.

### **NVIDIA A100-SXM4-40GB (sm_80)**

| Operation | Tera-Operations/s (TOPS) | Giga-Operations/s (GOPS) |
| :-------- | :----------------------- | :----------------------- |
| **ADD** | `0.597`                  | `596.5`                  |
| **MUL** | `1.303`                  | `1302.8`                 |

### **NVIDIA Tesla T4 (sm_75)**

| Operation | Tera-Operations/s (TOPS) | Giga-Operations/s (GOPS) |
| :-------- | :----------------------- | :----------------------- |
| **ADD** | `0.119`                  | `118.7`                  |
| **MUL** | `0.253`                  | `253.4`                  |


* Achieving 1.3 Tera-Operations/sec for exact rational multiplication - 
 faster than hardware floating-point on the same GPU while maintaining 
 mathematical perfection.



---
## Why Exact Computation?

Eliminate floating-point errors in:
- Financial calculations
- Engineering simulations  
- Scientific computing
- AI/ML training
- Any application where precision matters
---

## Try It Now in Google Colab (No Install Needed!)

Click the links below to run a live demo of WarpFrac on a real NVIDIA GPU. (Download The 4 Warpfrac Files From The Releases Folder First, You Need Them For The Colab Demo! Make sure you run the demo using a T4/A100 GPU runtime!)

* **[Run on NVIDIA A100 (sm_80)](https://colab.research.google.com/drive/1_SkNBhIuaPKxpV_sR03KARBqv18wlN-z?usp=sharing)**
* **[Run on NVIDIA T4 (sm_75)](https://colab.research.google.com/drive/1fEjF9ZdXFeDjiIXqqXXoekVbg3U5-QMF?usp=sharing)**

## Use Cases

- Financial modeling with exact decimal arithmetic
- Engineering simulations without error accumulation
- Scientific computing with verifiable results
- AI/ML training with perfect reproducibility


## Requirements For Personal Machines

* **An NVIDIA GPU running on a Linux operating system.**
* Python 3.x
* NVIDIA CUDA Toolkit compatible with your driver.

**Note:** This software is not compatible with macOS or Windows as it requires direct access to NVIDIA hardware. For a live demonstration, please use the Google Colab links above.
---

## License & Terms of Use

This software is distributed under a binary only license. **Source code is not available, and reverse engineering, decompiling, or disassembling the binaries is strictly prohibited.**

* Please see the `LICENSE.txt` file for copyright information.
* Refer to `EULA.txt` for the full End-User License Agreement.
* **Note**: External publication of benchmarks requires prior written consent from me, Evan Wesley, The Smartest Idiot Alive.


### API Overview
```python
import warpfrac

