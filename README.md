# WarpFrac — High-Performance GPU Fraction Arithmetic

WarpFrac is a Python library providing GPU-accelerated arithmetic (CPU coming soon!) for fractions using precompiled, high-performance CUDA kernels. This is a **binary-only evaluation release** and is not open-source.

---

## Performance Benchmarks

The following benchmarks were recorded on an **NVIDIA A100 (sm_80)** GPU.

| Operation | Tera-Operations/s (TOPS) | Giga-Operations/s (GOPS) |
| :-------- | :----------------------- | :----------------------- |
| **ADD** | `0.495`                  | `494.6`                  |
| **MUL** | `1.298`                  | `1297.3`                 |

---

---

## Try It Now in Google Colab (No Install Needed!)

Click the links below to run a live demo of WarpFrac on a real NVIDIA GPU. (Download The Files From The Releases Folder First!)

* **[Run on NVIDIA A100 (sm_80)](https://colab.research.google.com/drive/1_SkNBhIuaPKxpV_sR03KARBqv18wlN-z?usp=sharing)**
* **[Run on NVIDIA T4 (sm_75)](https://colab.research.google.com/drive/1fEjF9ZdXFeDjiIXqqXXoekVbg3U5-QMF?usp=sharing)**

---

## License & Terms of Use

This software is distributed under a binary-only license. **Source code is not available, and reverse engineering, decompiling, or disassembling the binaries is strictly prohibited.**

* Please see the `LICENSE.txt` file for copyright information.
* Refer to `EULA.txt` for the full End-User License Agreement.
* **Note**: External publication of benchmarks requires prior written consent from me, Evan Wesley, The Smartest Idiot Alive.
